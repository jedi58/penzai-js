# penzai-js
A JavaScript library to create a collapsible tree with optional checkboxes without the use of jQuery, and uses ARIA descriptions. It is named after the ancient Chinese art of depicting artistically formed trees, other plants, and landscapes in miniature; similar to Japanese bonsai.

## Demo
See [CodePen](https://codepen.io/jedi58/pen/dPXvawW) for an interactive demo

<img width="356" height="168" alt="image" src="https://github.com/user-attachments/assets/6a395079-738d-47e5-b2b1-336978652ba0" />

```html
<ul id="categoryTree">
  <li>Fruits
    <ol>
      <li>Apple
      <ol>
        <li>Golden Delicious</li>
        <li>Granny Smith</li>
      </ol>
      </li>
      <li>Banana</li>
    </ol>
  </li>
  <li>Vegetables
    <ol>
      <li>Carrot</li>
      <li>Broccoli</li>
    </ol>
  </li>
</ul>
<script src="penzai.min.js"></script>
<script>
    const tree = penzai(document.getElementById('categoryTree'), {
        checkboxes: false,
        expandAll: false // starts collapsed
    });
</script>
```
