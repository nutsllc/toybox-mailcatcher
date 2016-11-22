# Toybox Mailcatcher

This is the smallest docker image (162 MB) for [MailCatcher](https://mailcatcher.me/) based on [Alpine Linux](https://alpinelinux.org/)

## What is the mailcatcher ?

>MailCatcher runs a super simple SMTP server which catches any message sent to it to display in a web interface. Run mailcatcher, set your favourite app to deliver to smtp://127.0.0.1:1025 instead of your default SMTP server, then check out http://127.0.0.1:1080 to see the mail that's arrived so far.

## Run container

```bash
docker run -p 1025:1025 -p 1080:1080 -itd nutsllc/toybox-mailcatcher
```

After running a container, you will go to ``http://hostname:1080/`` to see WEB Interface and send mail through ``smtp://hostname:1025``.
