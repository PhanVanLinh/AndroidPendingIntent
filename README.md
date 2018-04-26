# AndroidPendingIntent

`PendingIntent` wrapper `Intent`.  `PendingIntent` grant permission to a foreign application to use the contained Intent
If you give the foreign application an Intent, it will execute your Intent with its own permissions. But if you give the foreign application a PendingIntent, that application will execute your Intent using your application's permission

### Major use
- Handle action in `Notification`
- Handle action in `Widget`
- Declaring an intent to be executed at a specified future time (`AlarmManager`)

### Create Pending Intent
- `PendingIntent.getActivity()` for an Intent that **starts an Activity**.
- `PendingIntent.getService()` for an Intent that **starts a Service**.
- `PendingIntent.getBroadcast()` for a Intent that **starts an BroadcastReceiver**.

### Reference
https://stackoverflow.com/a/4812421/5381331  
https://developer.android.com/guide/components/intents-filters