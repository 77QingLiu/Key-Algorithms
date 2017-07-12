# Key-Algorithms


## Algorithms 4th edition�ص��㷨������ˢ�⣬��ϰ��׼�����Զ��кܴ������

### ��1�� ����
&emsp;[1.1 �������ģ��](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter1_1)<br />
&emsp;[1.2 ���ݳ���](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter1_2)<br />
&emsp;[1.3 ���������к�ջ](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter1_3)<br />
&emsp;[1.4 �㷨����](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter1_4)<br />
&emsp;[1.5 �����о���union-find�㷨](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter1_5)<br />
### ��2�� ����
&emsp;[2.1 ���������㷨](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter2_1)<br />
&emsp;[2.2 �鲢����](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter2_2)<br />
&emsp;[2.3 ��������](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter2_3)<br />
&emsp;[2.4 ���ȶ���](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter2_4)<br />
&emsp;[2.5 Ӧ��](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter2_5)<br />
### ��3�� ����
&emsp;[3.1 ���ű�](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter3_1)<br />
&emsp;[3.2 ���������](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter3_2)<br />
&emsp;[3.3 ƽ�������](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter3_3)<br />
&emsp;[3.4 ɢ�б�](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter3_4)<br />
&emsp;[3.5 Ӧ��](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter3_5)<br />
### ��4�� ͼ
&emsp;[4.1 ����ͼ](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter4_1)<br />
&emsp;[4.2 ����ͼ](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter4_2)<br />
&emsp;[4.3 ��С������](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter4_3)<br />
&emsp;[4.4 ���·��](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter4_4)<br />
### ��5�� �ַ���
&emsp;[5.1 �ַ�������](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter5_1)<br />
&emsp;[5.2 ���ʲ�����](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter5_2)<br />
&emsp;[5.3 ���ַ�������](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter5_3)<br />
&emsp;[5.4 ������ʽ](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter5_4)<br />
&emsp;[5.5 ����ѹ��](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter5_5)<br />
### [��6�� ����](https://github.com/jimmysuncpt/Algorithms/tree/master/src/com/jimmysun/algorithms/chapter6)<br />
### [�ٷ�����](https://github.com/jimmysuncpt/Algorithms/tree/master/src/edu/princeton/cs/algs4)<br />


### ��һ��ˢ���С���ӣ�

leetcode 104�⣬�ҵ������������ȣ�����ǵ� 3.3binary search tree�������height��code���Ϳ���˲��д��bug free��solution�ˡ�


������3.3binary search tree�������height��code��

```java
/**
* Returns the height of the BST (for debugging).
*
* @return the height of the BST (a 1-node tree has height 0)
*/
public int height() {
    return height(root);
}
private int height(Node x) {
    if (x == null) return -1;
    return 1 + Math.max(height(x.left), height(x.right));
}



//������104��Ľⷨ��



/**
* Definition for a binary tree node.
* public class TreeNode {
*     int val;
*     TreeNode left;
*     TreeNode right;
*     TreeNode(int x) { val = x; }
* }
*/
public class Solution {
    public int maxDepth(TreeNode root) {
        if (root == null) return 0;
        return 1 + Math.max(root.left, root.right);
    }
}

