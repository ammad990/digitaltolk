# Digital Tolk
I have few comments to add in this readme file about the shared code;
## Booking Controller
The naming convention looks good and code is properly indented, however there is lot of code written in a single Controller file i.e. BookingController
- The Job related methods should be added to a separate JobController. This will help in keeping the code clean and meaningful to read with the use of proper Controller name.
- The same things shoudl be done with the notifications method. These methods should be added separately in a NotificationController
- The role id's should be loaded from database table, having proper schema defined for users and their roles.

## Booking Repository
There is a more and more code written in Booking repository which should be cleaned and optimized.
- The history related functions should be added separately in HistoryRepository
- The job relevant functions should be added to JobRepository
- Push notifications should be added to NotificationRepository,
- $this->mailer should be replaced with Laravel built in Notifications.
- The code is indented properly but messed by misiing different codes in a single file.
