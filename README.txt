🎂  HAPPY BIRTHDAY SURPRISE PAGE  🎂
=====================================

A little single-page website that:
  1. Opens with party poppers 🎉
  2. Reveals a photo + a lovable quote on each tap 💖
  3. Ends with a big birthday blast + your wish 🎆

Everything is in ONE file: index.html. No internet, no install needed.


-------------------------------------------------
QUICK START (3 steps)
-------------------------------------------------
1. Put your photos in THIS folder, named:
       photo1.jpg
       photo2.jpg
       photo3.jpg
       ... and so on, in the order you want them shown.

   The page finds them automatically and stops at the first
   missing number. Want 8 photos? Just go up to photo8.
   (.jpg, .jpeg, .png, .webp and .gif all work.)

2. Open index.html — double-click it, or drag it into a browser.
   (Even with NO photos it works, using placeholders, so you
    can preview the whole experience first.)

3. Send it to her! (See "Hosting" below.)


-------------------------------------------------
PERSONALIZE IT
-------------------------------------------------
Open index.html in any text editor. Near the top of the <script>
section there's a block marked:

    ✏️  EDIT ME

Change these:
  • name          -> her name
  • openingNote   -> the teasing line on the very first screen
  • quotes        -> one line per photo (in order)
  • fallbackQuotes-> extra lines used if you have more photos than quotes
  • inPersonWish  -> the heartfelt pause shown after the last photo
  • finalTitle    -> the big finale headline ({name} is filled in for you)
  • finalMessage  -> your heartfelt closing note
  • giftIntro     -> the line above the gift choices
  • gifts         -> the list of gifts she can tap (emoji + label)
  • giftConfirm   -> shown after she picks ({gift} is filled in with her choice)
  • photoDir      -> leave "" if photos are in this folder.
                     Use "photos/" if you keep them in a subfolder.

THE JOURNEY, IN ORDER:
  opening (teasing note) -> photos + quotes -> heartfelt "wish I was there"
  pause -> birthday blast -> "pick your gift" screen. When she taps a gift
  it lights up and confirms — she can tell you what she chose. 🎁

Tip: Every photo always gets a caption. If you have more photos than
quotes, the extras borrow from fallbackQuotes automatically.


-------------------------------------------------
HER GIFT CHOICE REACHES YOU — EMAIL + WHATSAPP 💌💬
-------------------------------------------------
When she picks a gift and taps "Send my gift to him 🎁":
  • EMAIL  -> sent to you silently, automatically.
  • WHATSAPP -> opens with the message pre-typed to your number; she
               taps Send once.
Then she sees: "Your gift option has been processed and safely sent
to me 💖 ✓"

(A) EMAIL  ->  web3formsKey   (one-time, free, ~1 minute)
    1. Open  https://web3forms.com
    2. In the "Create your Access Key" box, type your email
       kartheesan468@gmail.com  and submit.
    3. Web3Forms emails you an Access Key (a long code like
       "a1b2c3d4-...."). Open that email and copy the key.
    4. Open index.html in a text editor. In the EDIT ME block find:
             notify: {
               ...
               web3formsKey: "",
       and paste your key inside the quotes:
               web3formsKey: "a1b2c3d4-....",
    5. Save. Done — her choice now emails you automatically.
    (If you leave it blank, email is simply skipped.)

(B) WHATSAPP  ->  uses WhatsApp's official Click-to-Chat. No key needed.
    Her tap opens WhatsApp with the message ready to your number
    (918220062151); she presses Send.
    To change the number: EDIT ME block -> notify -> whatsapp
    (full international form, no "+", e.g. 918220062151).

WHY IT WORKS THIS WAY: a static webpage has no secret place to store a
login/token, so it can't log into your email or WhatsApp by itself.
Web3Forms is a free relay that sends the email for you. WhatsApp's
fully-automatic Cloud API would need a private server (a token can't
live in a public page), so we use WhatsApp's own Click-to-Chat, which
is free and needs just her one tap.

NOTE: Instagram DM isn't possible — Instagram gives webpages no way to
send DMs. Email + WhatsApp are the reliable routes.


-------------------------------------------------
OPTIONAL: BACKGROUND MUSIC 🎵
-------------------------------------------------
1. Put a song file (e.g. song.mp3) in this folder.
2. In the EDIT ME block, set:  music: "song.mp3"
The song starts on the first tap and there's a 🔊 button (top-right)
to mute/unmute.


-------------------------------------------------
HOSTING (so she can open it from her phone)
-------------------------------------------------
Easiest options (all free):

• Netlify Drop:  https://app.netlify.com/drop
  Drag this whole BDay folder onto the page — you instantly get a
  link you can text her.

• GitHub Pages:  create a repo, upload these files, enable Pages.

• Or just AirDrop / send the folder and have her open index.html.

Note: keep index.html and the photo files together in the same
folder (or the same photos/ subfolder) so the links stay valid.


-------------------------------------------------
CONTROLS
-------------------------------------------------
Tap / click anywhere  -> next photo
Space / Enter / →     -> next photo (on a computer)
"Replay 💖" button    -> start over

Have fun, and happy celebrating! 🎈
