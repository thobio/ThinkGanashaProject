#  DataModel

### Login api
    
    Needed to add a new key  ** is_reviewer ** of Bool type.

### Report Flag

    To Report a Flag to entries We need a new api.

        1. entries_id : String
        2. selected_reason : String
        3. flag_message : String
        4. flaged_user_id : String

### New Entry List

    New Entry list  waiting for approval from the reviewers.

        1. entries_id : String
        2. image_url  : String
        3. title_text : String
        4. des_text   : String
        5. entries_user_id : String

### Flaged Entry list 

    Flaged Entry list is the list of entry that other user reported flag.

        1. entries_id : String
        2. image_url  : String
        3. title_text : String
        4. des_text   : String
        5. entries_user_id : String
        6. flag  : [Flag]
        
            > Flag

            1. flag_id : String
            2. flag_reason : String
            3. flag_message : String
            4. flag_user_id : String

###  Flaged EntryList 

    Flaged Entry remove the flaged entry or remove the flag from the entry

        1. entry_id : String
        2. remove_all_flag : Bool
        3. remove_entry : Bool
        4. reviewer_id : String

### New Entry Approval or not

    New Entry Approval or not 

        1. entry_id : String
        2. approval_entry : Bool
        3. reviewer_id : String