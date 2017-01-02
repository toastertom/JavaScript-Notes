# Node Properties ([Back To Index](https://toastertom.github.io/JavaScript-Notes/))

## A **Node** is an interface from which a number of DOM types inherit, and allows these various types to be treated (or tested) similarly.

---

**node.parentNode** read-only property returns the parent of the specified node in the DOM tree.

#### Syntax

```

parentNode = node.parentNode

```

#### Example

```

if (node.parentNode) {
  // remove a node from the tree, unless
  // it's not in the tree already
  node.parentNode.removeChild(node);
}


```

---
