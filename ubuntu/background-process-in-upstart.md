# Running a background process in upstart mode in Ubuntu

You dont have to put the `&` symbol to put the process in background. It will work without that. Sample configuration:

```start on startup

respawn

setuid deploy
exec php /var/www/document_service/current/daemon/archiver/run_archiver.php```

`start on`: Ensures that on reboot of the system the script starts
`respawn`: Ensures that if the process is somehow killed, it starts again
`setuid deploy`: Sets the user that runs the process to deploy
`exec`: Executes the command
