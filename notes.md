**Class Notes**

    • Goal: Learn the most important and fundamental technologies for a web service by building a startup
    • Technologies
        HTML - Structure
        CSS - Style
        JavaScript - Interaction
        Service - Web service endpoints
        Database/Login - Persisted app and auth data
        WebSocket - Data pushed from server, chat
        React - Web framework
    • Tips:
        ○ Don't worry too much about looks. They can always be easily revisited but functionality is the more important goal
        ○ Put in consistent effort!! Set aside time each day (for me, ~2 hours). Cramming leads to a poor product
            § Remember that you want to continue this startup well after this class is over to continue demonstrating your abilities
        ○ Don't do too much with UI right now. Keep UI to a minimum and know that you can always add more UI after the class is over 
        ○ Similarly, don't worry about too many features. You will add more features when class is over
    • Throughout the semester, we'll use the Simon Startup example to learn individual technologies

        • Structure and Goals for the Class
            ○ We're going to learn Front End and Back End web development
            ○ We're going to learn to make an application for a startup company
                § What could I do to change people's lives?
            ○ HTML, CSS, JavaScript, React, Node.js, Mongo
            ○ We're going to participate in Active Learning
        • Goal of the class: to learn how to learn these skills (the skills themselves will be obsolete soon if not already)
        • Course
            ○ You don't need to read everything; Don't get caught in an accumulation of ignorance. Understand everything as you go
        • Learning Web Programming
            ○ The biggest skill you can develop in the class is learning how to learn
        • How to get help
            ○ Ask google, ChatGPT, discord
    
        • How to be a good software engineer
            ○ Improvements in 4 categories:
                § Capable: The more intimate and deep your understanding of a technology, the more you will be able to take advantage of its capabilities and maximize your productivity
                § Creative: The ability to think outside the box and create well-sculpted, efficient code
                § Collaborative: Social skills; the ability to work with others to create a project together
                § Curious: Wanted to know the 'why' behind the 'how', constantly learning and upgrading your knowledge in new things
        • Discord
            ○ You should use the channel that is most appropriate for your discussion.
            ○ Do not ask questions in multiple channels.
            ○ Only use general if it really is not specific to another channel.
            ○ If you are replying to someone multiple times then reply in a thread and not in the channel.
        • How to ask questions (from canvas):
        
            Clearly define and phrase your question. Sometimes this alone will give you an answer.
            Use the clearly defined question to research for more information.
            Give ample background. Assume the person you are asking is not looking at your computer, doesn't know what you are working on, and doesn't know what you know. Because they don't. Saying "It doesn't work" provides no value. It isn't even a question. Instead give the background in as much detail as possible. Explain what you tried already and what the result was.
            Screenshots and captured output is helpful.
            Give a reproduction path.
            Use proper grammar and proofread your question.
            Respond to feedback.
            Give thanks even if you didn't find the help you were hoping for.
            Here is a good template to follow when asking a question:
            
            When working on assignment A, I was successfully able to do 1, 2, and 3, but then I did B, as instructed by C, and got the result D, with an error of E. I was expecting F. I thought maybe G or H might be the problem, but I saw that J already tried that without success as discussed here on K. Any help is greatly appreciated.
            
        • Startup
            ○ Goal: Learn the most important and fundamental technologies for a web service by building a startup
            ○ Technologies
                HTML - Structure
                CSS - Style
                JavaScript - Interaction
                Service - Web service endpoints
                Database/Login - Persisted app and auth data
                WebSocket - Data pushed from server, chat
                React - Web framework
            ○ Tips:
                § Don't worry too much about looks. They can always be easily revisited but functionality is the more important goal
                § Put in consistent effort!! Set aside time each day (for me, ~2 hours). Cramming leads to a poor product
                    □ Remember that you want to continue this startup well after this class is over to continue demonstrating your abilities
                § Don't do too much with UI right now. Keep UI to a minimum and know that you can always add more UI after the class is over 
                § Similarly, don't worry about too many features. You will add more features when class is over
                
            ○ Throughout the semester, we'll use the Simon Startup example to learn individual technologies
        
    
        • Some helpful POSIX commands
            ○ echo - Output the parameters of the command
            ○ cd - Change directory
            ○ mkdir - Make directory
            ○ rmdir - Remove directory
            ○ rm - Remove file(s)
            ○ mv - Move file(s)
            ○ cp - Copy files
            ○ ls - List files
            ○ curl - Command line client URL browser
            ○ grep - Regular expression search
            ○ find - Find files
            ○ top - View running processes with CPU and memory usage
            ○ df - View disk statistics
            ○ cat - Output the contents of a file
            ○ less - Interactively output the contents of a file
            ○ wc - Count the words in a file
            ○ ps - View the currently running processes
            ○ kill - Kill a currently running process
            ○ sudo - Execute a command as a super user (admin)
            ○ ssh - Create a secure shell on a remote computer
            ○ scp - Securely copy files to a remote computer
            ○ history - Show the history of commands
            ○ ping - Check if a website is up
            ○ tracert - Trace the connections to a website
            ○ dig - Show the DNS information for a domain
            ○ man - Look up a command in the manual
        
            ○ | - Take the output from the command on the left and pipe, or pass, it to the command on the right
            ○ > - Redirect output to a file. Overwrites the file if it exists
            ○ >> - Redirect output to a file. Appends if the file exists

    • What is a technology stack?
        ○ The collection of different technologies used to run a web service
        ○ These are usually 'stacked' in the sense that they are layered (web framework -> web services -> backend technologies)
    • What is a web server?
        ○ A physical computer located in a massive storage warehouse, in this case one of Amazon's
    • What is TLS?
        ○ A standard encryption protocol used to authenticate, encrypt and protect information exchange over the internet (typically TCP). 
        ○ Based on a handshake system where a 'secret' is shared to then encrypt and authenticate further exchange of information (try 'curl' with -v to see handshake in action)
        ○ Replaced its predecessor SSL (sometimes still referred to as SSL)
    • What is a web certificate?
        ○ Issued to verify that a certificate owner is the actual owner of a domain.
        ○ Let's Encrypt revolutionized this process making it accessible and free to obtain such a certificate
    • What is Caddy?
        ○ Web server + configuration management system that will act as a gateway (reverse proxy/connection manager) to our various services in our project
        ○ Important Caddy files
            § "~/Caddyfile" - Configuration files
                □ Contains the routing procedure definitions for incoming HTTP requests 
            § "~/public_html" - HTML files
                □ The directory of files that Caddy serves up when requests are made to the root server
                □ Contains index.html (typically defined the home page/the first thing the user sees connecting to the website)

The Console
    • What are POSIX commands?
        ○ A standardized set of commands like 'pwd' and 'ls' that work with POSIX compliant consoles (like Git Bash) to interact with the computer system
        ○ Useful+common POSIX commands:
            § pwd - Print working directory
            § echo - Output the parameters of the command
            § cd - Change directory
            § mkdir - Make directory
            § rmdir - Remove directory
            § rm - Remove file(s)
            § mv - Move file(s)
            § cp - Copy files
            § ls - List files
            § curl - Command line client URL browser
            § grep - Regular expression search
            § find - Find files
            § top - View running processes with CPU and memory usage
            § df - View disk statistics
            § cat - Output the contents of a file
            § less - Interactively output the contents of a file
            § wc - Count the words in a file
            § ps - View the currently running processes
            § kill - Kill a currently running process
            § sudo - Execute a command as a super user (admin)
            § ssh - Create a secure shell on a remote computer
            § scp - Securely copy files to a remote computer
            § history - Show the history of commands
            § ping - Check if a website is up
            § tracert - Trace the connections to a website
            § dig - Show the DNS information for a domain
            § man - Look up a command in the manual
        ○ Chain commands
            § | - Take the output from the command on the left and pipe, or pass, it to the command on the right
            § > - Redirect output to a file. Overwrites the file if it exists
            § >> - Redirect output to a file. Appends if the file exists
            § Example: "ls -l | grep ' Nov ' | wc -l" lists the files in a directory, pipes it into grep to search for files created in Nov, and pipes that into wc to count the number of files found with a date of Nov.
        ○ Keystrokes
            § CTRL + R - Does a convenient 'reverse search' on already-typed commands to quickly access and reuse them
            § CTRL + C - Kills the current command process
Editors
    • What is the Live Server Extension (VSC)?
        ○ Commonly used to develop web applications, serves up project in the local browser for convenient feedback
CodePen
    • What is CodePen?
        ○ A simple, interactive coding sandbox site for experimenting with immediately-rendered code 
HTML
    • What is HTML?
        ○ Stands for Hypertext Markup Language
        ○ Originally created as a successor to simple text files for sharing readable content on the internet
    • HTML Input
    
        Hello World
        
        ○ The above is technically valid HTML code, though it is clearly just plain text and doesn't take advantage of any of the features of HTML
            
        <p>Hello World</p>
        
        ○ The above now shows the text "Hello World" being represented as an HTML element (specifically a paragraph element) with delimiting tags of the form <something>, </something>
        
        <html>
          <head>
            <title>My First Page</title>
          </head>
          <body>
            <main>
              <p>Hello World</p>
            </main>
          </body>
        </html>
        
        ○ Now adding more structure, we see the <html> element representing the top-level page structure, the <head> element providing metadata about the page and page title, and the <body> element providing content structure, where its <main> element provides structure to the main body of content (as opposed to headers, footers, navigation content, etc).
        ○ Note that rendering this information will still render the exact same as our original "Hello World" text as we've only provided simple structure to our page
        ○ What are attributes?
            § Attributes describe specific details of HTML elements. For example, 
            <p id="hello" class="greeting">Hello world</p>
            Shows an example of the id attribute (giving a unique ID to an element) and the class attribute (designating the element as among a specific named group)
            § Another very common and useful attribute is the hyperlink attribute, implemented here (found within the necessary anchor element):
                <a href="https://byu.edu">Go to the Y</a>
        
        <!DOCTYPE html>
        <html lang="en">
          <body>
            <main>
              <h1>Hello world</h1>
              <p class="introduction">
                HTML welcomes you to the amazing world of
                <span class="topic">web programming</span>.
              </p>
              <p class="question">What will this mean to you?</p>
              <p class="assignment">Learn more <a href="instruction.html">here</a>.</p>
            </main>
          </body>
        </html>
        
        Renders as 
        
        
        
        ○ Note <!DOCTYPE html> is required to tell a browser what information to expect
        ○ What are some common HTML elements?
            § html	The page container
            § head	Header information
            § title	Title of the page
            § meta	Metadata for the page such as character set or viewport settings
            § script	JavaScript reference. Either a external reference, or inline
            § include	External content reference
            § body	The entire content body of the page
            § header	Header of the main content
            § footer	Footer of the main content
            § nav	Navigational inputs
            § main	Main content of the page
            § section	A section of the main content
            § aside	Aside content from the main content
            § div	A block division of content
            § span	An inline span of content
            § h<1-9>	Text heading. From h1, the highest level, down to h9, the lowest level
            § p	A paragraph of text
            § b	Bring attention
            § table	Table
            § tr	Table row
            § th	Table header
            § td	Table data
            § ol,ul	Ordered or unordered list
            § li	List item
            § a	Anchor the text to a hyperlink
            § img	Graphical image reference
            § dialog	Interactive component such as a confirmation
            § form	A collection of user input
            § input	User input field
            § audio	Audio content
            § video	Video content
            § svg	Scalable vector graphic content
            § iframe	Inline frame of another HTML page
        ○ How do we do html comments?
            § <!-- commented text --> uncommented text
        ○ How are special characters rendered?
            § Using the & escape with the proper entity (can be used to render any unicode char)
            Char	Entity
            &	&amp;
            <	&lt;
            >	&gt;
            "	&quot;
            '	&apos;
            😀	&#128512;
    • What are some HTML input elements?
        form            Input container and submission	   <form action="form.html" method="post">
        fieldset       Labeled input grouping	                <fieldset> ... </fieldset>
        input	       Multiple types of user input             <input type="" />
        select	       Selection dropdown	                 <select><option>1</option></select>
        optgroup   Grouped selection dropdown           <optgroup><option>1</option></optgroup>
        option	       Selection option	                               <option selected>option2</option>
        textarea     Multiline text input	                 <textarea></textarea>
        label	       Individual input label	                  <label for="range">Range: </label>
        output	       Output of input	                               <output for="range">0</output>
        meter	       Display value with a known range    <meter min="0" max="100" value="50"></meter>
    • 'Live Server' is hugely useful for first developing and later deploying website files
    • linux 'find' command
        □ e.x. find /path/to/search -type f -name "*.txt"

