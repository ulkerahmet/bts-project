# Binary Search Tree

Binary Search Tree (BST), her düğümün sol alt ağacındaki tüm değerlerin o düğümün değerinden küçük, sağ alt ağacındaki tüm değerlerin ise büyük olduğu bir ikili ağaçtır. Verilen diziye göre adım adım bir BST oluşturabiliriz:

1. **Root 7'dir:**
   - Root: 7

2. **5, 7'den küçük olduğu için soluna eklenir:**
   - ```
     7
    /
   5
   ```

3. **1, 7'den küçük ve 5'ten de küçük olduğu için 5'in soluna eklenir:**
   - ```
     7
    /
   5
  /
 1
   ```

4. **8, 7'den büyük olduğu için sağına eklenir:**
   - ```
     7
    / \
   5   8
  /
 1
   ```

5. **3, 7'den küçük, 5'ten küçük, 1'den büyük olduğu için 1'in sağına eklenir:**
   - ```
     7
    / \
   5   8
  /
 1
  \
   3
   ```

6. **6, 7'den küçük, 5'ten büyük olduğu için 5'in sağına eklenir:**
   - ```
     7
    / \
   5   8
  / \
 1   6
  \
   3
   ```

7. **0, 7'den küçük, 5'ten küçük, 1'den küçük olduğu için 1'in soluna eklenir:**
   - ```
     7
    / \
   5   8
  / \
 1   6
/ \
0   3
   ```

8. **9, 7'den büyük, 8'den büyük olduğu için 8'in sağına eklenir:**
   - ```
     7
    / \
   5   8
  / \   \
 1   6   9
/ \
0   3
   ```

9. **4, 7'den küçük, 5'ten küçük, 1'den büyük, 3'ten büyük olduğu için 3'ün sağına eklenir:**
   - ```
     7
    / \
   5   8
  / \   \
 1   6   9
/ \
0   3
     \
      4
   ```

10. **2, 7'den küçük, 5'ten küçük, 1'den büyük, 3'ten küçük olduğu için 3'ün soluna eklenir:**
    - ```
      7
     / \
    5   8
   / \   \
  1   6   9
 / \
0   3
   / \
  2   4
    ```

Bu adımlar sonucunda oluşan Binary Search Tree şu şekildedir:

```
     7
    / \
   5   8
  / \   \
 1   6   9
/ \
0   3
   / \
  2   4
```