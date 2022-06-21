1. justify-content
2. align-items
3. flex-direction
4. orde
5. align-self
6. flex-wrap
7. flex-flow
8. align-content

## 水平对齐元素

### **justify-content**

| flex-start    | 元素和容器的左端对齐。   |
| :------------ | ------------------------ |
| flex-end      | 元素和容器的右端对齐。   |
| center        | 元素在容器里居中。       |
| space-between | 元素之间保持相等的距离。 |
| space-around  | 元素周围保持相等的距离。 |

## 纵向对齐元素

### **align-items**

| flex-start | 元素与容器的顶部对齐。     |
| ---------- | -------------------------- |
| flex-end   | 元素与容器的底部对齐。     |
| center     | 元素纵向居中。             |
| baseline   | 元素在容器的基线位置显示。 |
| stretch    | 元素被拉伸以填满整个容器。 |

## 元素在容器里摆放的方向

### **flex-direction**

| row            | **元素摆放的方向和文字方向一致**         |
| :------------- | ---------------------------------------- |
| row-reverse    | 元素摆放的方向和文字方向相反（从右向左） |
| column         | 元素从上放到下                           |
| column-reverse | 元素从下放到上。                         |

**注意**：**当你调转行或列的方向后，flex-start和flex-end对应的方向也被调转了**。

**注意：当flex以列为方向时，justify-content 控制纵向对齐，align-items 控制横向对齐。**

## 设置单个元素的位置

### **order**

元素的属性默认值为0，可以设置这个属性为正数或负数。

order：1  ；     正数向flex-end方向移动；

order：-1 ；	负数向flex-start方向移动。

## 控制单个元素

### **align-self**

这个属性接受和`align-items`一样的值。

## 换行

### **flex-wrap**

| nowrap（默认） | 所有的元素都在一行。     |
| :------------- | ------------------------ |
| wrap           | 元素自动换成多行         |
| wrap-reverse   | 元素自动换成逆序的多行。 |

## 方向与换行的缩写属性

### **flex-flow**

**flex-direction**和**flex-wrap** 的缩写属性，这个缩写属性接受两个属性的值，两个值中间以**空格**隔开。

例如：**flex-flow: row wrap** ；

## 行与行之间隔

### **align-content**

| flex-start    | 多行都集中在顶部。         |
| ------------- | -------------------------- |
| flex-end      | 多行都集中在底部。         |
| center        | 多行居中。                 |
| space-between | 行与行之间保持相等距离。   |
| space-around  | 每行的周围保持相等距离。   |
| stretc        | 每一行都被拉伸以填满容器。 |

**这可能有些容易混淆，但`align-content`决定行之间的间隔，而`align-items`决定元素整体在容器的什么位置。只有一行的时候`align-content`没有任何效果。**