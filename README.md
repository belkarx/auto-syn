# auto-syn
Automatically grabs a digest of grades from Synergy and emails to some recipient(s)

## Setup
Grab browser driver (chromedriver for example) following the instructions in `chromedriver_install.txt` or (for firefox) `geckodriver_install.txt` [note: if you're using geckodriver, change the code at `#firefox` so that the firefox binary is not specifically specified - I was using firefox's development/beta build so I needed to explicitly state the location of the binary however that is unnecessary for typical firefox]

Things to be edited (sending/receiving email, etc) can be found by searching for `#CHANGE HERE` comments.

2 environment variables can be set: `PY_PASS` and `PY_EMAIL_PASS`

The program can be run with `python3 auto.py`

Remember to `pip3 install` selenium and bs4.

Also, your sending email should be outlook (I'd recommend just making a new email), and POP3 should be enabled in the settings.

You can set an anacron job to run this every once in a while if you wish.

## Sidenote
This isn't intended to be "good" code, but it should work, and does its job as a utility script decently well 
