---
up:
  - "[[Ideaverse Pro Hangar]]"
related: []
created: 2022-05-11
modified: 2023-08-25
---

# Ideaverse Pro 2.0

## Hotfix (2025-04-29)

- Moved the [[Calendar]] note into the `Maps` folder and updated the `Collection` property with `Views` and `Maps` in order to surface it in queries.

_Released 2025-04-16_

So much has evolved, oh my. We can only effectively talk about the high-level changes. 
## Headlines 
- Official reveal of "**Wayfinders**"
    - You'll be able to fly around your notes faster than ever before with these navigation aids. LYT Wayfinders are fully integrated into this ideaverse.
- New and powerful **High-Context Views**
    - See multiple kinds of notes in compelling, high-context views to significantly improve your sensemaking. From your idea notes to your calendar notes, these views increase your ability to find what you need, exactly when you need it. 
- A completely reimagined **Home Pro**
    - Now with clean, beautiful, and easy-to-edit wayfinders. 
- All improved and expanded "**Collections**"
    - **22** ~~13~~ Collections to help you prioritize your efforts, manage your meetings, cultivate your ideas, and organize your books, movies, the people in your life, and tons more including meetings, quotes, events, ideas, etc.
- New **Quick Capture** workflow
    - Use this workflow to capture new ideas faster than before. 
- **3+ Hours of BRAND NEW Online Lessons **with walkthroughs and examples.
    - 16 practical online lessons get you feeling capably in your new home. 
- A **full in-vault tutorial** for the ACE Folder Framework. 
    - 17 in-vault lessons and 1 hour of recordings to guide how ACE works.
- **3 Choose Your Own Adventure Learning Experiences: **_The best way to learn how to use linked notes is to actually use linked notes to learn!!_
    - LYT 101 for Orientation: 16 interlinked notes
    - LYT 201 for Ideation: 28 interlinked notes
    - LYT 301 for Organization: 21 interlinked notes
- All improved **Templates**
    - 42 ~~28~~ **pre-made Templates** that work perfectly with all the collections. There are some powerful ones I can't wait for you to experience.
- **Ideaverse Zero** - a clean "done for you" Ideaverse without my notes but with all of my settings to give you a solid foundation.
- **All my Personal Settings**
    - **155+** ~~137~~ Custom Callouts
    - Custom keyboard settings
    - Theme & Appearance modifications
    - Installed Plugins
- **2+ Hours of Additional Recordings** Additional lessons and example notes to help you understand how they support me day to day and how they might help you.
- Brand new theme: **Soft Paper**
	- A well-balanced theme that is easy on the eyes.
- 12 Months of Updates.
- Plus so much more. 



# Ideaverse Pro 1.5

## Hotfix (2024-08-05)

- Fixed the [[Map Template (Collections)]] to properly load in queries by replacing the `Views` property with the `Collections` property.


## Changes

- Added **Home Pro Basic**.
  - It's a simple and clean home note. It's the non-flashy, but highly functional alternative to [[Home Pro]]. It's intentionally easy to edit, so we expect you to edit it to your personal tastes—just try to keep the formatting simple!
- Formally introducing **Folder x**.
  - _The "x" folder stands for "extras"_. It works incredibly well in Obsidian and in your computer's file folder system as well.
  - It's a release valve, an easy way to tuck away those "extra" types of notes, such as "notes about notes" (meta notes, vault-related notes), utility notes, archived notes, and less immediately relevant "placeholder folders" that, while not overly important now, still serve you as a tucked away reminder of a topic or area of simmering or potential interest.
  - Keen observers with notice that some folders have been shuffled around as a result.
- Supercharged the **Maps** note.
  - Now with views to quickly and powerfully find your most important notes. Views include:
    - Maps that are "Collections"; Maps that are "Views"; Atlas maps by rank; Calendar maps; Effort maps; All the maps by folder; My favorite handmade maps; and a General list of my favorite maps.
- Installed the highly customized [[Soft Paper Theme]].
  - This alternative to the default Prism theme will put you in a calmer and more reflective state of mind.
- **Added handy links to online lessons** into each relevant note.
  - Now, notes that have a relevant online lesson for Ideaverse Pro have links directly to the lesson.
- **Metadata power shift** from tags to properties.
  - Eliminated `#map` and `#map/view`. Replaced it by linking with the `collection` property to `[[Maps]]` and, when appropriate, `[[Views]]` too.
  - Eliminated `#source` and all of its nested tags like `#source/book`. Replaced it by linking with the `collection` property to `[[Sources]]` and, when appropriate, notes like `[[Books]]` too.
    - Ideaverse Pro now simply has the `collection` property link to their subtypes like `[[Papers]]`, `[[Music]]`, etc
  - Quotes saved through `#source/quote` were turned to use inline metadata `quote::`, which are now viewable in the bottom [[Quotes]] dynamic view.
  - We also added a new property to all map notes called `mapState` that you'll see displayed in the dynamic views within the Maps note.
- New map: **Sources**!
  - Sources is such a huge thing, we created a parent-level collection for all the sources you may wish to collect. This note comes with the dynamic views for Books, Movies, and Series. We've also added dual views for "All Sources" using the new `collection` property, along with a backup version that points to the `Atlas/Sources` folders—so you have options if depending on if you prefer folders or properties.
- Improved the dynamic view in [[Quotes]].
  - Now it shows a dynamic view of inline quotes, which searches for any line prefixed with `quote:: `
- Your property metadata now auto-sorts when you click away.
  - Added a pretty neat Auto-sort effect, that auto-sorts key properties to also be in the ideal order. Learn more at [[Properties#Auto sorting properties]] when saving or switching notes using the Linter plugin
- Improved the dynamic view in [[Meetings]].
  - Now it shows inline meetings, which searches from `meeting::` at the start of a line.
- Improved the dynamic views in [[Collections]].
- Simplified the [[Library]] note's formatting.
  - By taking the text out of the callouts, we are encouraging you to actually edit the Library note to make it your own.
- Tucked away a new folder called `Master Keys` within the x folder.
  - It has a few special notes that help auto-suggest values when you're filling out specific property values for notes on Maps and People.
- Gave the graph view more life in the light mode Prism theme.
  - Dots, Home notes, Collections, and Maps now pop with variations of the core LYT colors for a more dynamic graph in light mode.

### All Changes

- Removed {{title}} from query add-on logic to only use `[[]]` so they still work regardless of note title change
- Fixed some example source notes with improper values which led to unexpected sorting results in views
- Removed Nick's folder paths in Dataview queries
- Added queries to show new and updated notes in this note
- Creating a new daily note using the QuickAdd log feature creates a note in `Notes` instead of `2022` folder
- Fixed movie and book search scripts not working
- Updated Ideaverse Pro Glossary note to link to Classification note for more details
- Renamed all X folders to lowercase x
- Fixed `Courses` example notes having the `type` property set to `Courses` instead of `collection`, which made them not show in queries
- Properties would have an error in the `plot` property if the plot text returned had double quotations mark, so they've been removed from the template
  - The specific example used was from searching `Black Mirror` and choosing the 2011 option

## New Notes in this Version

```dataview
list
from ""
where contains(version, "1.5")
sort file.name
```

## Major Note Updates

```dataview
TABLE updates as "Updates"
FROM ""
WHERE updates
sort file.name
```

---

# Ideaverse for Obsidian 1.0

_Released 2023-08-30_
**Headlines**

- Introduced the [[Home]] note with ACE head spaces.
  - Provide multiple examples of
  - Provided a basic ARC Framework (Add, Relate, Communicate) for developing ideas into outputs.
- Introduced the [[ACE Folders]].
  - Provided ACE with multiple notes and examples.
- Introduced a working system for [[Efforts]] based on intensities.
  - Provided "Efforts" with multiple examples.

**Details**

- 310 notes
- Improved several data views to power up your navigating experience.
- Did general clean-up.
- Changed the name of the kit from LYT Kit to Ideaverse for Obsidian because Ideaverse evokes the connected, yet wide open nature of notes and ideas.
  - Further, this release is called Ideaverse for Obsidian. But the name opens the door for other versions such as of Ideaverse for Organizations and Ideaverse for XYZ. So the name change allows the principles to naturally transcend the tool.

# LYT Kit 7 - Release Notes

_Released 2022-09-13_

**Headlines**

- Vintage Home note
- 16 empowered maps in the Home note
- ACCESS folders streamlined to 10 folders
- Introducing "Efforts"

**Details**

- 286 notes
- Vintage Home note.
  - Remade the Home note to match the original version that brought me so much joy.
- 16 empowered maps in the Home note. Rebuilt every map for clarity and power.
  - Thinking MOC, Inbox, Notebox, Outbox, Daily Notes
  - Library, People MOC, Sources MOC, Concepts MOC
  - Efforts, Plan and Review
  - Health MOC, Finance MOC, Life Map, LYT Kit and Meta PKM
- Streamlined ACCESS folder structure for an easier start.
- Introduced "Efforts" as an alternative to "Projects".
  - Added the "Efforts" map to the Home note.
- Improved several data views to power up your navigating experience.
- Did general clean-up.

---

# LYT Kit 6 - Release Notes

_Released 2022-05-11_

- 309 notes
- ACCESS folder structure
- Revised many of the notes for clarity
- Added Callouts explaining the broken links in some notes leading to parts of my personal PKM unavailable in Ideaverse for Obsidian
- Recorded a series of e-mail lessons exploring some PKM fundamentals as well as working within the ACCESS folder structure to offer a bit more guidance in exploring this vault
- Added several new MOCs, indexes, and data views
- General clean-up
