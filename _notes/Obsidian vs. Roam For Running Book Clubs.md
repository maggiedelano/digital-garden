---
title: Obsidian vs. Roam For Running Book Clubs
---

# Obsidian vs. Roam For Running Book Clubs
This is a version of a note I wrote in our shared Obsidian vault as part of Dan Allosso's [Obsidian Book Club](https://danallosso.substack.com/p/obsidian-book-club-the-dawn-of-everything) on the *Dawn of Everything* by David Graeber and David Wengrow. I'm removing comments from others just because I don't have their permission to share them. I'm focused here specifically on the tools, not so much how the specific book club was run.

## Obsidian has more challenges getting started with multiplayer
I'm starting with the friction points because this is what you tend to notice at the start of the club, but there are plenty of advantages discussed in the next section!

### Lack of user specific customization
There is a lack of individual customization of vaults, requiring "shell" vault for your own customization to not influence other people. In Roam you can choose which settings apply to everyone or only certain people, for example a standard CSS that can be modified by individuals (though javascript always has to be opted into for security reasons). This is very easy for new users because the organizers choose the defaults and the user can leave it alone (unless they want to use custom functionality).

Also, the other issue is that given everyone is sharing the same `.obsidian` folder, **anyone** can change the settings for **everyone**, which makes it difficult to have strong defaults for new users, which would be nice.

### Lack of clear landing page
There is no "landing page" or shared sidebar, compared with the shared sidebar in Roam and the daily notes page as a landing page. One potential solution to this is to use the [Homepage](https://github.com/mirnovov/obsidian-homepage) plugin or starred notes, but we did not try it in the first Obsidian book club.

### Difficulty using the same page at the same time
It can be fun in Roam to all write together on the same page. This works well and sort of like a Google doc so long as you don't have too many users at the same time (like over 100). This is not really possible in Obsidian with the Dropbox merge conflicts. The Dropbox merge conflicts also come up sometimes when someone is just viewing a file, even if they don't actively edit it. This could be an issue with Dropbox rather than Obsidian though. 

### Lack of user sandbox
It's a little harder to isolate people's personal notes from one another because in Obsidian it makes sense to work with a folder of atomic notes not a single personal page like in Roam. This means we could have a dozen "Chapter 1" notes which is kind of annoying. I recommend using a prefix or suffix in personal notes as Dan and I have done e.g. ``[[MKD Journal]]``.

### Hard to see what's been updated recently
This is something that Roam has issues with as well (easily seeing what has changed since you last visited), but you can handle this easily in Roam by linking to the Daily Notes Page, which is the first thing that shows up when a user signs in to the graph. With all the comments distributed throughout the vault, this is likely an issue. The way we got around this in the book club was using the [Changelog](https://github.com/badrbouslikhin/obsidian-vault-changelog) plugin. This worked well, but because it runs only on one person's computer it is not "always on." Each person could set up their own instance in their shell vault if they wanted to, though. 

### Hard to link files to other people, especially when using shell vault
There isn't an easily available and consistent URL you can link to like you can in Roam. This mostly comes up in live discussions where you want to make reference to a specific note or block. You can use `obsidian://` links, but these are tied to a vault, so everyone would have to name their book club shells the same thing for them to work. Another alternative is to use the Dropbox URL, or you just paste the wikilink and the other person pastes that in and clicks it. 

## Obsidian May Encourage More Contribution to Shared Knowledge

### Obsidian is faster and easier for browsing and organization
Especially with the addition of folders, Obsidian is much easier to browse and navigate because it's much clearer what it is in there. It is also much easier to avoid overwhelm by realizing the root folder is getting out of control and creating homes for notes organically. Roam can be kind of a black hole and needs to be structured carefully for things not to get lost.

### Obsidian encourages writing in prose
As Obsidian is not an outliner (unlike Roam), it encourages you to write in prose. This helps make your future notes much more organized, but has the trade off that it can be harder to organize complex concepts or notes with a lot of content (though folding and the outline view in the side panel helps a lot).

Possibly because Obsidian encourages you to write in prose, it seems much more feasible to me for multiple people to easily contribute to a shared knowledge base. In Roam Book Club we often turn on a feature called immutable blocks, which prevents users from editing blocks created by other users. This was necessary because people would unintentionally delete the work of others, and Roam only has hourly backups. Dropbox seems better suited to handling potential lost information, so long as the merge conflicts are not so bad.

### Obsidian has a better graph view
The graph view allows one to easily see which pages have not been created, for example, which you could then consider populating.

### Page back links in Obsidian do not create files
This is really nice because you can find pages that have been linked to but are not created yet in the `[[` menu or using the Graph view, but they do not clutter up the file explorer. In Roam Book Club, we have to ban people from creating their own pages for the first few weeks because it becomes too much of a mess, especially because pages are case sensitive (unlike in Obsidian). Another reason for this is because Roam treats pages and tags the same. I did not use tags in Obsidian much, so anyone using them did not interfere with me, and those tags can also easily be namespaced to not be too disruptive. 

### File Portability
One other advantage of Obsidian is that these markdown files are very easy to export and save later. This means they can easily be backed up to personal vaults or moved to future vaults. You can do this in Roam but it requires exporting, and if you don't use name spaces it's a pain in the butt to get all the files you want. (I guess this is the same constraint as using folders, though).

## Overall Thoughts
I think Obsidian has a lot of promise especially if the goal is to attempt to create a shared knowledge base. Care should be taken to help onboard new users, especially given that the best experience in Obsidian is more dependent on plugins and customization compared with Roam. 

I've been impressed with how much people have been able to organically contribute to the vault structure so far, and also contribute to notes in the Glossary etc., without many hiccups that I can tell. One consideration is that this book is very different from the books we've read in Roam Book Club so far, so it's possible we'd get that sort of engagement reading this book too, but I think it's easier to jump in in Obsidian. People are sometimes afraid of "messing things up" in Roam.