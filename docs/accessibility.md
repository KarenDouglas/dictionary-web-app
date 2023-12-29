# Accessibility Checklist

Ensuring that your HTML is readable to screen readers is essential for creating an inclusive and accessible web experience. Here is a checklist of best practices to make your HTML more accessible:

1. **Use Semantic HTML:**
   - Use semantic HTML elements (e.g., `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`) to properly structure your content. Semantic elements convey the meaning and structure of the content to both browsers and screen readers.

2. **Provide Descriptive Text:**
   - Use descriptive and meaningful text for links, buttons, and form elements. Avoid generic phrases like "click here" or "read more." Instead, use text that describes the purpose or destination of the link or button.

3. **Add Alternative Text to Images:**
   - Include descriptive alternative text (`alt` attribute) for all images. This text should convey the essential information or function of the image. Decorative images can have an empty or null alternative text (`alt=""`).
   ```html
   <img src="example.jpg" alt="A descriptive text about the image">
   
4. **Use ARIA Roles and Attributes:**
- Accessible Rich Internet Applications (ARIA) roles and attributes can enhance the accessibility of dynamic content. For example, use `role="button"` for elements that act like buttons.

```html
<div role="button" tabindex="0">Click me</div>
```

5. ***Ensure Keyboard Accessibility***
- Ensure that all interactive elements (links, buttons, form controls) are navigable and operable using a keyboard. Use the tabindex attribute when necessary, but be cautious and avoid changing the default tab order unless absolutely necessary.

```html
<a href="#" tabindex="0">Clickable Link</a>
```

6. ***Provide Focus Indication***
- Ensure that users can easily see where keyboard focus is on the page. Use CSS to provide a visible focus indicator for links and form controls. Be mindful of users who navigate with a keyboard.

```css
:focus {
  outline: 2px solid #007bff; /* Add your preferred focus styling */
}
```

7. ***Create Accessible Forms***
- Label form controls using the `<label>` element and associate them with their corresponding input fields. Use the for attribute in the label to link it with the id of the form element.

```html
<label for="username">Username:</label>
<input type="text" id="username" name="username">
```

8. ***Ensure Logical Heading Structure***
- Use heading elements (`<h1>`, `<h2>`, etc.) to create a logical structure for your content. Headings provide an outline of the document's hierarchy and help screen reader users navigate through the content.

9. ***Test with Screen Readers***
- Regularly test your website with popular screen readers like NVDA (NonVisual Desktop Access), JAWS (Job Access With Speech), or VoiceOver. This allows you to experience your content from the perspective of users who rely on screen readers.

10. ***Provide Transcripts for Multimedia***
- For multimedia content like audio or video, provide text transcripts or captions. This ensures that users with visual or hearing impairments can access the information.

