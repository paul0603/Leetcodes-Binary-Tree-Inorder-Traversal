# Leetcodes-Binary-Tree-Inorder-Traversal
## *Description: Given the root of a binary tree, return the inorder traversal of its nodes' values.*
**Thought**:
It is intuitive to apply recusive approach.
Since inorder traversal start from left, we first travel to leftnode, then itself, and last, the right node. So the code may look like
```c++
vector<int> inorderTraversal(TreeNode* node)
  If node.leftnode != null /* travel to left node */
    v_left=inorderTraversal(node.left)
  
  v_left=v_left.push_back(node.value) /* current node */
  
  If node.rightnode~= null /* travel to right node */
    v_right=inorderTraversal(node.rightnode)
    
  return v_left+v_right  /* append right to left */
 ```
