# expeditiondrive
sketch-a-thon webpage

The Amendment for future use of the website:

HTML:
 Amended:
1. Seperate HTML and CSS in two files (you can use the same CSS file for another HTML file, and easier to read too.) 

2. Amended the spelling of "boxx" into "box" (avoid future confusion in case you forget the reason of using "xx")

3. deleted unused tag <script>

4. changed the tag <article> into <main> and it no longer contains <footer> tag in it  (for structure reason)

5. the class ".purple" is amended into ".-purple" to signified that it is an utility class.

CSS:
  Amended:
1. Any reason for using empty ruleset? (i made all of them into comments)

https://stackoverflow.com/questions/32464170/visual-studio-code-css-error-do-not-use-empty-rulesets

2. universal selector "*" replace the line "body, html, p, h1, h2, h3, h4, h5, h6 {margin: 0; padding: 0;} /* zeroing */", Universal selector "*" will apply in the whole styling in the webpage.
But, need to add (ul{padding: 10px 0px 10px 40px}) in CSS file

Note: "box-sizing: border-box" is just to make things easier to adjust with the sizing of box.

3. Moving "html, body { font-family: 'Raleway', sans-serif; }" into universal selector "*" for the same reason in Number 2.

4. Deleted the color:white in <h1>, since body already has the color:white

5. Amended (section .purple {color: #D283ED;}) into (.-purple {color: #D283ED;}), to make it reusable.

Issue-uncleared:

1. the line "a, a:visited {color: #9146D4}" is conflicted with ".ex-links a, .ex-links a:visited{color: white}"

2. the line "a:focus, a:hover {color: white;}" is conflicted with".ex-links a:hover, .ex-links a:focus {color: #9146D4}"

3. Why the h1 margin-top is -.2.5rem? It covered a part of the text in h1 in my screen.

4. the .ex-links font-size: 1.34em, would suggest to change to REM, just in case you want to expand the footer and accidentally used em as font size in .ex-links future parent tag.

5. Suggest to give class name to each of the element instead of styling directly on the tag. 

a)To improve readability (take less time to remember where is "foward p" if it has a common name, maybe i would put class "explanation" instead)

b) less risk of error because if the specificity of the class name compared with "forward p". i mean in future you might want another <p> tag in forward ID with different styling. 

6. is there a reason for using header h1 instead of just h1? same issue with section .important, footer .ex-link and others. 

7. Optionally, you can choose on whether you want to use the comments under the body tag and delete the rest of the CSS styling under it to make your CSS shorter. But more work need to be done if for example, you want to change the font style of h1 to other style, you need to amend at the combined class and the individual class below. 