- point1  
    - subpoint1  
        - sub-subpoint1  
- []  
- point2  
    - **subpoint2**  
        - sub-subpoint2 
        - ![image2.webp](https://docs-api-qa.cloudlabs.ai/repos/raw.githubusercontent.com/ankitSpektra/LabGuideNew/main/text-input-demo/images/image2.webp)

# Test
# Comprehensive Nested List Test

## Test 1: Basic Nested Unordered Lists
- Level 1 item 1
    - Level 2 item 1
        - Level 3 item 1
        - Level 3 item 2
    - Level 2 item 2
- Level 1 item 2
    - Level 2 item 3

## Test 3: Mixed Ordered and Unordered
- Unordered level 1
    1. Ordered level 2
        - Unordered level 3
        - Unordered level 3
    1. Ordered level 2
- Unordered level 1

## Test 4: Images in Nested Lists
- Point 1
    - Subpoint with text
        - ![Sample Image](https://via.placeholder.com/150)
        - Another subpoint after image
    - Subpoint 2
- Point 2
    - ![Image at level 2](https://via.placeholder.com/200)

    ## Test 4: Images in Nested Lists
- Point 1
    - ![allclouds_image.png](https://docs-api-qa.cloudlabs.ai/repos/raw.githubusercontent.com/Rabin-spektra/Demo-Repo/main/196993496zpeJ/images/allclouds_image.png) 


## Test 5: Links in Nested Lists
- Main point
    - Check out [Google](https://www.google.com)
        - Nested link: [GitHub](https://github.com)
        - Plain text after link
    - Another point with [link](https://example.com)

## Test 6: Bold and Italic Formatting
- **Bold text at level 1**
    - *Italic text at level 2*
        - ***Bold and italic*** at level 3
        - Regular text with **bold word** inside
    - Text with *italic word* inside

## Test 7: Code in Lists
- Regular text
    - Code example: `console.log('Hello')`
        - Inline code: `const x = 10;`
        - Another point
    - More `code` examples

## Test 8: Combined Formatting
- **Bold point** with *italic*
    - Link: [Visit Site](https://example.com) with **bold**
        - Image and text: ![icon](https://via.placeholder.com/50) `code snippet`
        - All together: **Bold** *italic* `code` [link](https://test.com)

## Test 9: Deep Nesting (4+ levels)
- Level 1
    - Level 2
        - Level 3
            - Level 4
                - Level 5 (if supported)
                

## Test 10: Multiple Items at Each Level
- Item 1A
    - Item 2A
        - Item 3A
        - Item 3B
        - Item 3C
    - Item 2B
        - Item 3D
        - Item 3E
    - Item 2C
- Item 1B
    - Item 2D
    - Item 2E

## Test 11: Text Before and After Lists
This is a paragraph before the list.

- List item 1
    - Nested item 1
    - Nested item 2
- List item 2

This is a paragraph after the list.

## Test 12: Complex Real-World Example
- **Prerequisites**
    1. Install [Node.js](https://nodejs.org) (version 16+)
    1. Install `npm` or `yarn` package manager
        - For npm: `npm install -g npm@latest`
        - For yarn: `npm install -g yarn`
    1. Clone the repository
- **Configuration**
    - Create `.env` file
        - Add `API_KEY=your_key_here`
        - Add `DATABASE_URL=your_db_url`
    - Run setup: `npm run setup`
- **Running the App**
    1. Development mode: `npm run dev`
    1. Production mode: `npm run build && npm start`
        - Check logs: `tail -f logs/app.log`
        - Monitor at [http://localhost:3000](http://localhost:3000)

## Test 13: Lists with Images and Links Combined
- Product Features
    - ![Feature 1](https://via.placeholder.com/100)
        - Learn more: [Documentation](https://example.com/docs)
        - See **demo** at [Live Site](https://example.com/demo)
    - ![Feature 2](https://via.placeholder.com/100)
        - *New feature* with `beta` tag

## Test 14: Edge Cases
- Single item list
- List with empty nested level:
    - 
- List back to content
- **Multiple** *formats* `together` in [one line](https://test.com)
    - ![img](https://via.placeholder.com/50) **Bold** *italic* `code`

## Test 15: Checkbox Lists (if supported)
- [ ] Unchecked task
    - [ ] Nested unchecked
        - [x] Nested checked
    - [x] Another checked
- [x] Checked task