# Media-query

Hosted Link:- https://lok-ii.github.io/Media-query/

![Screenshot 2023-08-23 175045](https://github.com/Lok-ii/Media-query/assets/129180844/0116ac56-d0f7-479d-947a-a0fa77d32a34)

    HTML Description:
    
        <!DOCTYPE html>: This declaration defines the document type and version of HTML being used (HTML5 in this case).
    
        <html lang="en">: The opening tag of the HTML document. The lang attribute specifies the language of the content (English).
        
        <head>: This section contains metadata and links to external resources used by the webpage.
        
        <meta charset="UTF-8">: Sets the character encoding to UTF-8, which supports a wide range of characters and symbols.
        <meta name="viewport" content="width=device-width, initial-scale=1.0">: Specifies the viewport settings for responsive design. The width=device-width ensures the viewport width matches the device width, and initial-scale=1.0 sets the initial zoom level.
        <link rel="stylesheet" href="styles.css">: Links to an external stylesheet named "styles.css" for styling the webpage.
        <title>Media Query</title>: Sets the title of the webpage displayed in the browser's title bar.
        
        <body>: This section contains the visible content of the webpage.
        
            <main>: Defines the main content section of the webpage.
                <div class="container">: Creates a container for the main content.
                    <div class="image"></div>: An empty <div> used to display a background image.
                    <div class="content">: A <div> for textual content.
                        <h1>Certified Coffee <br> Courses</h1>: An <h1> heading with a line break for the title.
                        <p>: A paragraph with dummy text.
                        <p>: Another paragraph with dummy text.
                        <a href="">Freepik</a>: A link to "Freepik," though the href attribute is empty in this example.
                        <button>LEARN MORE</button>: A button element.

    CSS Properties Used:-

        body:
            font-family: sans-serif;: This rule sets the default font family for the entire webpage to a sans-serif typeface, which is a clean and modern choice for text.

        main:
            background-color: black;: This sets the background color of the main element to black, providing a dark background for the content.
            display: flex;: This makes the main element a flex container, allowing its child elements to be aligned and spaced using flex properties.
            justify-content: center; and align-items: center;: These properties center the child elements both horizontally and vertically within the main element.
            width: 100%; and height: 100vh;: These properties ensure that the main element covers the entire viewport width and height.

        .container:-
            background: linear-gradient(#fff 24%, #f1c40b 10%);: This creates a linear gradient background, transitioning from white (#fff) to a yellowish color (#f1c40b). The percentages control the gradient's color transition points.
            max-width: 50rem; and width: 100%;: These properties control the maximum width and full width of the .container element.
            height: 33.5rem;: Sets the height of the .container element.
            color: black;: Defines the text color for the content within the .container.
            display: flex; and align-items: center;: Similar to earlier, these properties center the child elements within the .container.

        .image:
            background-image: url(./assets/coffee.png);: Sets the background image of the .image element to "coffee.png" located in the "assets" folder.
            background-size: contain;: Makes sure the background image is contained within the .image element.
            background-repeat: no-repeat;: Prevents the background image from repeating.
            width: 100%; and height: 25.625rem;: Sets the width to full width and the height of the .image element.
            flex-shrink: 3;: Allows the .image element to shrink when needed in case of limited space.

        .content:-
            text-align: center;: This property centers the text content horizontally within the .content element.
            display: flex;, flex-direction: column;, justify-content: center;, align-items: center;: These properties, combined, center the child elements vertically and horizontally within the .content element and arrange them in a column.
            width: 100%;: Sets the width of the .content element to full width.
            flex-shrink: 3;: Allows the .content element to shrink when necessary, but to a lesser extent than the .image element.

        .content h1:
            margin-top: 4rem;: Adds a top margin of 4rem to the <h1> element within the .content element.
            font-weight: 700;: Sets the font weight of the <h1> element to a bold (700) weight.

        .content p:
            line-height: 1.2rem;: Sets the line height of the <p> elements to 1.2 times the font size, improving readability.
            font-size: 0.75rem;: Sets the font size of the <p> elements to 0.75rem.
            font-weight: 700;: Sets the font weight of the <p> elements to bold (700).

        .content p a:
            .content p a selects anchor (<a>) elements within <p> elements inside .content.
            font-size: 0.75rem;: Sets the font size of links within paragraphs to 0.75rem.
            color: black;: Sets the color of the links to black.

        button:
            color: white;: Sets the text color of the button to white.
            background-color: black;: Sets the background color of the button to black.
            height: 1.875rem; and width: 9rem;: Sets the height and width of the button.
            font-size: 0.6rem;: Sets the font size of the button text to 0.6rem.
            letter-spacing: 0.1rem;: Adds spacing between letters for the button text.
            border: none;: Removes the border around the button.

        Media Queries:
            @media only screen and (max-width: 571px):
            
                This media query applies styles when the screen width is 571px or narrower.

                .container:
                
                    flex-direction: column; switches the flex direction to vertical stacking.
                    align-items: center; centers child elements horizontally.
                    height: 100%; makes the container take the full height of the viewport.
                    max-width: 100%; ensures the container's maximum width matches the viewport's width.
                    padding: 0; removes any padding.
                
                .image:
                
                    width: 50%; reduces the width of the image section to 50% of the container.
                
                .content p:
                
                font-size: 0.8rem; increases the font size of paragraphs.
                font-weight: 600; changes the font weight to semi-bold.
                line-height: 1rem; adjusts the line height for improved spacing.
                
            @media only screen and (min-width: 571px) and (max-width: 769px):
                
                This media query applies styles when the screen width is between 571px and 769px.
                .image:
                margin-top: 2rem; adds a top margin to the image section.
                margin-left: 5rem; adds left margin for spacing.
                max-width: 100%; ensures the image's maximum width matches the container's width.
                
            @media only screen and (min-width: 769px):
            
                This media query applies styles when the screen width is 769px or wider.
                .container:
                padding: 0.5rem 3rem 0 6rem; adds specific padding to the container for better spacing.
