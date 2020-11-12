# Bootstrap Containers

## Containers

Containers are the building block of Bootstrap.

All visible material should be in a container.

```html
<body>
  <div class="container">
    ...
  </div>
  ```

  Two types of containers

  * container: Width may change for elements
  * container-fluid:  Always 100% of the maximum width

## z-index

Containers have a z-index.  This allows elements to be on top of each other.  

High numbers are on top (visible)

Low numbers are behind (hidden) if they overlap a high number