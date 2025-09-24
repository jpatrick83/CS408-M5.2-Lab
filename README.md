# web-dev-starter

The project was a first look into Accessibility for HMTL.

## Getting Started

To get started, clone this repository (https://github.com/jpatrick83/CS408-M5.2-Lab.git) and run the following commands:

```bash
npm install
```
This will install the necessary dependencies for the project.

It is recommended to use the VSCode Live Server extension to run the project
locally. There is no need to run a build process or refresh the page manually. Additionally,
you do not need to setup a local server to run the project.

## Development

The only problem of me and the lab was a little time consuming as this is my first time working with Accessibility and finding the time to complete it.

## Accessibility Lab Answers

Color
The text is difficult to read because of the current color scheme. Can you do a test of the current color contrast (text/background), report the results of the test, and then fix it by changing the assigned colors?

Body text- 
   Contrast ratio ≈ 6.6:1 (pass)

Main headings
   Contrast ratio ≈ 11.2:1 (pass)
   
   White on green (#008000 default CSS green) → ratio ≈ 1.4:1 ❌ Fails (very poor readability).
   White on #ff80ff → ratio ≈ 1.8:1 ❌ Fails (also poor)

Nav bar
   Contrast ratio ≈ 13.6:1

Buttons
   Contrast ratio ≈ 12.6:1

Comments background
   Contrast ratio ≈ 9.2:1

Foreground	Background	Ratio
white on rgb(19,19,141)	16.6:1	
white on #4075b2	7.5:1	
white on #1a237e	13.9:1	
#0c0c0c on #4075b2	12.6:1	
#2a2a2a on rgb(19,19,141)	12.9:1	
#2a2a2a on #d9d9f9 (table)	12.8:1	
#2a2a2a on #def (odd row)	10.5:1	
#004d40 on #fdfeff (nav links)	12.4:1		
white on #000000 (submit)	21:1	
white on #333 (submit/show-hide)	12.6:1	

Semantic HTML
1.The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.
    We are able to focus on must of the elements but headers and the paragraph text are not reachable.

2. Can you update the article text to make it easier for screen reader users to navigate? There are two many breaks and not 
   setup to use <p> correctly.

3. The navigation menu part of the site (wrapped in <div class="nav"></div>) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.
Note: You'll need to update the CSS rule selectors that style the tags to their proper equivalents for the semantic headings. Once you add paragraph elements, you'll notice the styling looks better.
 "nav" should be listed as <nav>

The Images
The images are currently inaccessible to screen reader users. Can you fix this? We can add alt="description" to image for readers.

The Audio Player
The <audio> player isn't accessible to hearing impaired (deaf) people — can you add some kind of accessible alternative for these users? we can add a transcript of the file.
The <audio> player isn't accessible to those using older browsers that don't support HTML audio. How can you allow them to still access the audio? We can provide and way
to download the file.

The Forms
The <input> element in the search form at the top could do with a label, but we don't want to add a visible text label that would potentially spoil the design and isn't really needed by sighted users. How can you add a label that is only accessible to screen readers? We can user a aria-label

The two <input> elements in the comment form have visible text labels, but they are not unambiguously associated with their labels — how do you achieve this? Note that you'll need to update some of the CSS rule as well

Adjust the CSS slightly (gap, align-items, min-width) to ensure labels and inputs are visually clear and inputs remain usable on smaller screens.

The Show/Hide Comment Control
The show/hide comment control button is not currently keyboard-accessible. Can you make it keyboard-accessible, both in terms of focusing it using the tab key and activating it using the return key? Yes all we would need to do is user the <button></button>

The Table
The data table is not currently very accessible — it is hard for screen reader users to associate data rows and columns together, and the table also has no kind of summary to make it clear what it shows. Can you add some features to your HTML to fix this problem? we can add <table summary> and scope to get the read definition.

Other Considerations?
Can you list two more ideas for improvements that would make the website more accessible?
add “Skip to main content” link
Keyboard-accessible media controls for audio/video


## Testing

To run the tests for the project, run the following command:

```bash
npm test
```
