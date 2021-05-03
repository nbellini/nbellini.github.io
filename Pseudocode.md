# Plans for L8R (Long-term Reminders)

## Platform
I need to figure out which platform is going to be best for building my long-term project reminder.

Options:
I've being doing some research and although there were several options for python-based software, I am more interested in Apple's Xcode feature. I'd love to have a very simple app to run on my phone.

A difficulty is that I will have to learn Swift to code in it, but apparently it's an easy language to pick up.

## Code
Assuming this will work, I'm going to start thinking through what I want coded.

First, there will need to be an engine that you can enter your parameters into. These parameters would include:
- Title of goal
- Length of goal (start/end dates)
- Frequency of Reminders
- Task time

The Title would be defining the term, so probably just:

title = input("Name of Project: ")

or something. I might need to use strings or prints.

Length:

start date = date(input("mm/dd/yyyy"))
end date = date(input("mm/dd/yyy"))
length = ({end date} - {start date})
I'll need to look up the swift code to convey what I mean above.
If this gets too difficult, I may change it to:
length = int(input("Enter how many days you'd like your project to last: "))

Frequency:
reminders = int(input("Please enter the amount of times you would like to get reminded a week: "))

I'll need to figure out how to use this number to take {length}/x times a week

Maybe, if I do the second length idea, I can just do:
frequency = (({length}/7)*{reminders})

And that should give me the number of total reminders for the whole goal duration.  

Task Time:
duration = int(input(Enter how long you would like each reminder to be: ))

I will only end up needing this variable if I'm able to incorporate a timer for the beginning and end of the task! This would include two pop-up windows with an interval between them of the above duration.

Then, the whole app would take what was entered, generate, and schedule them.

## Sources I'm pulling from
I now need to look what I can actually find with swift code on github.  

I really just have no idea where to find useable code in these repositories. There's so many files that I don't know really what I'm looking for.

## Re-adjusting
Okay, looking at the app developer for Apple, I thought it would be template based, but now I realize I've greatly overreached my capabilities. Instead, I've re-examined some python codes on GitHub and found one I really like that includes texting the reminders: https://github.com/TwilioDevEd/appointment-reminders-flask
I think this could be a good way to include the timer! Instead of using an app pop-up, I can just send text messages.

Turns out the above is also too advanced, so now I really like this one: https://github.com/jonahar/google-reminders-cli
Seems like I can add some programming to adjust it well too my needs as listed above!

## Office Hour
So, in the office hour you really helped me figure out how to open the above Github, and after working through some error codes that I had to google, I got the application up and running and even added a reminder to my Google Calendar through it! Now all I have to do is figure out how to read the files and find where I need to edit to include to above pseudocode I've written.

## Editing the Code
So this is already tough because I'm not sure how to install everything, yet I'm relieved there's already a date and time reader installed, so it shouldn't be too difficult... I hope.

## Tutoring
So I worked with Kartika for an hour long tutoring session and she was able to help me figure out the basics of how the specific Google-reminders-cli code is working and where edits might be made, however she wasn't really able to offer specifics so now I'm working on

First error was "IndentationError: expected an indented block" which I was able to find a hanging if statement for
2nd error: "__init__() got an unexpected keyword argument 'end_dt'" so clearly my code needs some work

Got the time entry to work though I'm having difficulty getting it to work past just date entry.

## Office hour
Alright, so after meeting with you, I've decided to switch to building an HTML website since I don't think I'll be able to turn around this API with enough satisfaction or time. So, that being said...

# PROJECT 2: The website
I'll be building an html website for an upcoming songwriters collective I'll be starting in Nashville post-grad.

To start, I'll have to wipe clear what I have on it currently, and get started with a styles sheet.

Actually started by cleaning up the old work my group had done on the site for the in-class project.

Had to re-download and install everything on my new computer as well which took a while!

## Styles
Okay, I realized my styles sheet was actually a template which is great! I got it from w3schoools you referenced in class: https://www.w3schools.com/w3css/tryit.asp?filename=tryw3css_templates_startup

And here's what it looks like: https://www.w3schools.com/w3css/tryw3css_templates_startup.htm

## Assets

### General
Now I just need to start messing around importing assets for my business start-up.

Having a lot of fun so far, renamed the title and am working on adding a background photo to the website. I'm also gathering our assets such as examples of work, images, a logo for the group, and pictures of the team!

I'm also writing bios for the group.

Assets I'll be adding include: photos, audio, social links

### Photos
Had to go through Canva to find a solid free background photo: https://www.canva.com/templates/EADaifl2vus-blue-and-white-piano-music-youtube-channel-art/
  Had to add the image under the header - I had initally  gotten a little confused with placements within the styles section.

The photo is in and looks good, but I need to adjust the socials tag to be below it and get the text on the photo. Used: https://www.w3schools.com/howto/howto_css_image_text.asp to add a 'container.css' file to the projects to style the text on the photo. Finally got it to work after incorrectly nesting the text for a bit!

This is officially the first asset done!

### Audio
Now I need to reference the master list of HTML you gave us to remember how to include audio and this source: https://www.w3schools.com/html/html5_audio.asp

I'm going to steal the design used on the "about" section to apply to the 5 of us and our works.

I had to remember to pay attention to correctly labelling and referencing the audio, especially because I was working with both wav and mp3 files. Other than a quick syntax error I got this done pretty fast.

This is the second asset I have done!

### Social links
Adding these now, I figure I'll just work with the code around the social buttons and add href links. I've tried several things so far, adding the code within the (a) and (/a), (link), and href but so far no luck getting the links to actually hyperlink with the social buttons. After a lot of trial and error, I figured out to just switch the (i) to (a) and add an href link!

I also had to make sure to edit the bottom socials as well. I figured out how to add the SoundCloud social by altering the template and I'll also change the coding like  above.

Changing the padding so it's visible unlike how the socials currently sit on the edge of the picture. It looks great I'm so excited.

This asset is officially the third and final to be done!

## Re-design

### General
Going well so far, I've gone through the template changing stuff for the header but am having difficulty loading a background photo.

Editing out the pricing sections, renamed 'TEAM' to 'WRITERS' and 'PRODUCERS'

Added placeholder info for the assets, currently finished with formatting for above. Thinking of editing out certain features of the template like the promotion section and the skills section.
Okay, I kept promotion but deleted the skills and 'we know promo' sections

Filling in the contact information at the bottom.

Updated the about section to be a paragraph so the portfolio stands out more

Now I have to fix the home button links to href to the correct assets. Was able to do this after some searching and was able to find ID refs in each section I was able to update for the buttons I changed.

### Margins (as I know now)
Issue is now that rows are formatted to fit 4 boxes across, whereas I only have 3 and 2 so I'll have to mess around with the dimensions to fix that.
Need to add the photos for each team member now. Got them loaded really easily, but am not sure how to edit the styles to get the format correct, so I'm going to start looking through the linked styles sheets to find how to correctly alter the dimensions. It looks like messing around with the padding pre-sets is working, so I'll just keep doing some trial and error on that until it looks like what I want.

I've been working on this a lot now, but it's pretty hard to fix. I've tried lots of containers and style sheet changes but can't seem to get anything to work. Now trying to blindly guess the template coding to see if I can find their short cut to mess with the padding. Messing around with width didn't work, now going with adding lines of 'style="padding Xpx Ypx"' variations and seeing if it works. Didn't work, just shrunk the info on the card, but that just means I need to put the adjustment on the line of code with the card! Okay turns out that's where I already had it so I'm just checking around which container line will change the card. Omg, maybe I should put margin instead of padding! Padding was too big, reducing size.

Okay! I got the vertical line spacing down on the PORTFOLIO section, now I need to get it to adjust to the center properly. This is definitely the hardest part so far, but I think I'm finally really understanding certain formatting and styles pulls that I can work around with both the template and off the internet. Here's my source I used for an additional formatting container: https://stackoverflow.com/questions/4108726/how-to-spread-elements-horizontally-evenly. This didn't work!

I've definitely wanted Margins this whole time. Using this explanation from w3 where I got the template: https://www.w3schools.com/css/css_margin.asp I'll figure out how to get the spacing I want on both the PRODUCER and WORK/PORTFOLIO sections.

For the WORK section, I realized the coding including 'quarter' meant they spaced it by 4, so I was able to change it to 'third' and 'half' for my designs.

Went back and fixed margins/padding for social links and the company bio.

Now that I understand how to edit specific sections, I feel like I've really broken through exponentially with understanding how to design a website and edit in HTML. I'm super excited!

### Mail to links
Should've known I wouldn't be done yet, I've been going through the website and realized the last thing I need to add is our emails for contact, though that won't be too difficult as the cheat sheet, https://websitesetup.org/wp-content/uploads/2019/08/HTML-CHEAT-SHEET.png, includes the href Mailto code I saw earlier.
