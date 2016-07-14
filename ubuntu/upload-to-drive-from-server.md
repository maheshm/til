# Upload a file directly to Google Drive from a server

I had a huge directory that was to be shared with my client and I was having a limited internet access. I came across [this interesting project](https://github.com/prasmussen/gdrive). I downloaded the required version on the server, `chmod +x`ed it and ran `gdrive about`. It asked me to get a token from the web by pasting a generated URL. I ran `gdrive list` and voila, I could see all my Drive files listed in the terminal.

I `tar`ed the required directory, and ran `gdrive upload <filename>.tar.gz` and the file got uploaded in seconds. I saved my bandwidth and learned a new thing! :)
