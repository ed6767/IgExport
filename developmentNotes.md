# THESE NOTES ARE FOR REFFERENCE ONLY, they relate to the development of the project
Script using web Instagram dms
- use chromium based thing to send requests and pull JSON however possible
- then save them to a file 
- then extra options for export as plain text, html, pdf (converted from html)
- material and step based


Steps:
1. Login with Instagram
2. Select chat
3. Click start
4. Wait a while
5. Get exported chat log

Steps on backend:
1. Open cef at Instagram.com/accounts/login using android useragent
2. Inject JS on page (stored in res\js)
3. jS then makes requests like listing DMs and requesting messages


MISSING MESSAGE TYPES
- story replies
- sent stories
- added people
- removed people
- TODO FIRST

CHAT LOG UI
- using material web
- mainly chat but then can click and view info like open in Instagram ext.
- reverse the chat contents so it is in chronological order
- search
- more profile details
- printing, maybe for official police ext.


TODO:
- disappearing messages done
- gifs done
- finish ui
- replace new line with br
- match mp4 and jpg timestamps, so that thumbnail can be shown 
- audio messages in igexport viewer done
- printing/export
- browse media
- chat names and next page auto on login
- keep login option
- user support in igexport viewer
- SEARCH todo next
- fix long message issue (7000 message crash)
- export based 

order
allow replay
view once
stay in chat
sticker
gif
expired

raven_media = disappearing
unexpired-
raven_media.image_versions2.candidates[0].url = Image
raven_media.video_versions[0].url = VIDEO

IF URLS AREN'T THERE, EXPIRED.
VIEW ONCE CAN BE RETAINED ONLY IF NOT VIEWED IN APP.

animated_media = gif
DO NOT DOWNLOAD
src = animated_media.images.fixed_height.url


printing:
load page into body, flip and format, save html to array, clear body
done: render it all
