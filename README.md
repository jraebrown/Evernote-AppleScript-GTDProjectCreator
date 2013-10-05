Evernote-AppleScript-GTDProjectCreator
======================================

An AppleScript that looks for notes in a specified note. Useful for "Secret Weapon" or GTD-style Evernote usage.

I created this script to assist me in creating GTD project notes on my iPad.

My GTD set up works like this:
* All projects and actions go into a single notebook
* A note is created for each project
* Project notes have a tag assigned to them indicating that they're a project note, and not an action note
* Project notes also have the note link (Copy Note Link) set as the "Source URL" for the note
* An action relating to the project also has the "Source URL" field set to the link of the project note
* Single actions do not have the "Source URL" field defined

This set up gives me the the ability to search for all actions relating to a project. I copy the note link for the project, then perform a search for "sourceurl:"<project note link>""

However, the mobile clients for Evernote don't allow you to copy the note link for notes, only the *public* sharing link, which also makes the note public. I needed a way to be able to create a project note from the road. The first step is getting a script together that will create the project notes. This script looks for all notes in a separate notebook (called "Projects" in my setup). The script will then tag all the notes and set the source URL field to the note link, and then move them into my actions notebook.

My next step is to get the script executing via a scheduler so that it runs periodically.

I realize this script is fairly niche, but I'm throwing it over here anyway in case others find parts of it useful.
