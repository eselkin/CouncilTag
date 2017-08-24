# This is only for SM city council or HTML documents produced by the iqm2 auto-generated mechanisms
## Ideas for how to process data
0. Curl/get https://www.smgov.net/departments/clerk/agendas.aspx
1. Find table .'agendaTable' -> tbody
2. For Each tr 
    0. get date first <td>
    1. second <td> -> <a> :  parse for MeetingID
    2. Follow href from \#1 above
        * Get Meeting Group and type and date from spans with ids: having prefix "ContentPlaceholder1_lbl" and suffixes "MeetingGroup", "MeetingType", "MeetingDate" 
        * Search for 
            1. 
