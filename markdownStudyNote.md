title：markdown learning notes  
time:2020.10.1  
author:Wil909

***

### 1.Title

- The expression of the diffrent sizes of titles.

```
 1  # expresses the first level title.
 2  ## expresses the second level title.
 3  ### expresses the third level title.
 4  #### expresses the forth level title.
 5  ##### expresses the fifth level title.
 6  ###### expresses the sixth level title.
 ```
 Simply, only one # stands for the first level title.

 And since the number of # increases, the level of the title increases too.(Note:The level of a title is bigger, the size of the font is smaller!!)

 The style effects showed by the code block above are below.

 # # expresses the first level title.
 ## ## expresses the second level title.
 ### ### expresses the third level title.
 #### #### expresses the forth level title.
 ##### ##### expresses the fifth level title.
 ###### ###### expresses the sixth level title.

 And another way to mark the first level title is to use ===== , with marking the second level title using -----. (Rarely used)


---


 ### 2.Paragragh format.

- Paragragh  
   1.Adding ```2 spaces``` at the end marks the ending of the current paragragh.
   2.You can also use ```blank line``` to change a line.  
   Personally, I'm fond of the first way for the reason that it can show a neat style in the markdown file.

- Font  
  Markdown can use the several fonts below.
  ```
  1.  *Italics* or _Italics_
  
  2.  **Bold types** or __Bold types__

  3.  ***Bold italics*** or ___Bold italics___
  ```

  In person, I'd like to use the left style of writing, because in that way you have no need to  switch between Chinese and English to input the _.

  The  effects of the fonts are below.
  
  &emsp; *Italics*   
  &emsp; *Italics*  
  &emsp; **Bold types**  
  &emsp; **Bold types**   
  &emsp; ***Bold italics***  
  &emsp; ***Bold italics***

- The divider  
  You can use at least 3 of ```*,- or _``` to creat a line divider,without any other thing in the same line.  
  You can also insert space between the three symbols.  
  Any writing way below can creat a divider:
  
  ```
  1. ***

  2. * * *

  3. ******

  4. - - -

  5. -----------
  ```

  &emsp;&emsp;I would like the last writing style more.The reason is that thers is no need to swtich between Chinese and English or press shift.

  The effects are showed below:  
  
  ---  
  ---
  ---

- Strikethrough     
    
    &emsp;&emsp;It is funny.If you need to add a strikethrough on your words, you just need to add two ~~ on the both ends of the words.  
  &emsp;&emsp;(ps: the ~ must be English format.)    

  &emsp;&emsp;The instances are as below:  
  ```
  1 words

  2 ~~words~~
  ```

  The effects are showed below:

  &emsp;&emsp;words  
  &emsp;&emsp;~~words~~

- Underline

 &emsp;&emsp;There is no native grammar of the underline in markdown grammars, because it would cause conflicts with the default style of the 'link'.  
 &emsp;&emsp;So, if you really what to add a underline,you can use the HTML.  
 &emsp;&emsp;Instances are as below:

 ```
 1 words

 2 <u>words</u>
 ```

 Effects:
  
  &emsp;&emsp;words  
  &emsp;&emsp;<u>words</u>

- Footnotes    

  It is rarely used and difficule to write.  
  The footnotes is added to explain more clearly.    

  Instances are as belows:

  ```
  1 To creat a footnote is like this -> [^The footnote title]

  2 [^The footnote title]:the specific content
  ```

  Effects:  
  words [^footnotes]   
  [^footnotes]:author:wil909
 
 ------
### 3.List

 Markdown supports two lists, ordered lists and unordered lists.
 
 - Unordered lists  
   Use star(*), plus(+), or minus(-) as a mark of unordered lists.  
   I'd love to use the last ```minus(-)```to mark, for the reason as the same above.

   ```
    1 * The first item
    2 * The second item
    3 * The third item
    4 
    5 + The first item
    6 + The second item
    7 + The third item
    8
    9 - The first item
   10 - The second item
   11 - The third item
   ```

   Effects:  
     * The first item  
     * The second item  
     * The third item   
     + The first item  
     + The second item  
     + The third item  
     - The first item  
     - The second item  
     - The third item  
      
     &emsp; &emsp;This is becuase I have used a unordered list above, so the second level unordered list shows the hollow circle.    
       

 - Ordered lists
   
   Ordered lists use ```numbers with .```to simply stand for.

   ```
   1  1.The first item

   2  2.The second item

   3  3.The third item
   ```

   Effects:

   1. The first item
   2. The second item
   3. The third item

 - Nested lists
   
   Nested lists using in child lists just need to add 4 spaces or a tab:  
   ```In the thus writes the first level list```,```with a tab writes the second level list```,```with two tabs writes the third level list```. And so on...

   ```
   1  1. The first item
   2     - The first element nested in the first item
   3     - The second element nested in the first item
   4  2. The second item
   5     - The first element nested in the second item
   6     - The second element nested in the second item
   ```

   Effects:

  1. The first item  
     - The first element nested in the first item  
     - The second element nested in the first item  
  2. The second item  
     - The first element nested in the second item  
     - The second element nested in the second item  
  
  ---

### 4.Block
 
 &emsp;&emsp;The reference of the markdown block is to use character ```>``` at the start of the paragragh, and then there is a space character right following tightly.   
 &emsp;&emsp;If you would like to creat a new line in the block, it is needed to use two spaces:

 ```
 1  > The reference of the block.

 2  > The reference of the block.

 3  > The reference of the block.
 ```

 Effects:

 > The reference of the block.  
   The reference of the block.  
   The reference of the block.

 The block can also be nested, one > represents the outermost layer, two > represents the first nest, such as below:

 ```
 1  > The reference of the block

 2  >> The reference of the block

 3  >>> The reference of the block
 ```

 Effects:

 > The reference of the block
 >> The reference of the block
 >>> The reference of the block

 &emsp;&emsp;The block and list can  use nested with each other, and the best benifit is that it can keep the grammar style of the markdown grammar,instead of showing itself.

 ---

### 5.Code

 &emsp;&emsp;There are several expression ways of the code block.

 - Tick (')  
   If it is a function or fragments of code in a paragragh, you can use a tick to hug it.  
   For example:

   ```
   1  `printf()` function
   ```

   It is showed like:

    &emsp;&emsp;&emsp;&emsp;`printf()` function

 - Tab or four spaces
   
   &emsp;&emsp;Use a tab or add four spaces before every line, you can get a code block, as:

        private closeModal(){  
            let [fruit_id, weight] = [
               (this as any).current_fruit.fruit_id,
               this .fruit_weight
        ];
        this.$emit("hideModal");
        this.$emit("immediatePay",[{fruit_id,weight}])
        }

 - Use 3 ` to cover the words  before and after
   
   ```
   1  \```(In this position, you can set a language to show different color)
   2  private closeModal() {
   3   let [fruit_id, weight] = [
   4        (this as any)current_fruitfruit_id,   
   5         this.fruit_weight
   6   ];
   7    this.$emit("hideModal");
   8    this.$emit("immediatePay",[{fruit_id,weight}]);
   9   }
   10  \```

   ```

   ---

### 6.Link

  1.The simple writing way of link
   
   - Allocate a name for link

 ```
    1  [Link name](Link destination)
    2  for example:
    3  [Link of 菜鸟教程](http://www.runoob.com/markdown/md-link.html)
 ```

 Effects:

 &emsp;&emsp;[菜鸟教程](https://www.runoob.com/markdown/md-link/html)

 - Simply show the link  
     use `< ` and `>` to cover

   ```
   1  <https://www.runoob.com/markdown/md-link.html>
   ```

   Effects:

   <https://www.runoob.com/markdown/md-link.html>

 2.Advanced link  

   &emsp;&emsp;A link could be on behalf of a variable,with the direction of the variable in the end of the document:

   ```
   1  This link use 1 as the net variable[Google][1]
   2  This link use runoob as the net variable[Runoob][runoob]
   3  Then assign for the variable(net direction) in the end of the document
   4
   5  [1]:http://www.google.com/
   6  [runoob]:http://www.runoob.com/
   ```

 Effcts:

 This link use 1 as net variable [Google][1]  
 This link use runoob as net variable [Runoob][runoob]  
 And then assign for the variable(URL)
 
 
 [1]: http://www.google.com/
 [runoob]: http://www.runoob.com/
 ---

### 7.Photo
 The grammar format of a photo in markdown is as below:

 ```
 1   ![alt typeName](photo url)
 2   ![alt typeName](photo url "optional title")
 ```

 - With exclamation to start
 - Then write a `[]`,and inside write the alternative words of the photo
 - Then write a simple bracket with the url of the photo inside,and at last you can use `""` to cover some alternative words.
  
 ```
 1  ![RUNOOB icon](http:/static.runoob.com/images/runoob-logo.png)
 2
 3  ![RUNOOB icon](http://static.runoob.com/images/runoob-logo.png "RUNOOB")
 ```

 Effects:

 ![憨憨](/images/IMG_6901.jpg)

 ![憨憨](/images/IMG_6904.jpg)
 ![憨憨](/images/IMG_6916.jpg)
 ---

### 8.Form
 
 &emsp;&emsp;When using markdown to make a form,`|` is needed to divide different cells, and `-` is used to divide form head and other line.

 ```
 1  | Form head 1 ｜ Form head 2 |
 2  |--|--|
 3  |cell|cell|
 4  |cell|cell|
 ```

 Effetcs:    

 |Form head 1|Form head2|
 |--|--|
 |cell|cell|
 |cell|cell|

 And you can set the alignment of the sells (in the division line)

 - `-:` set right alignment
 - `:-` set left alignment
 - `:-:` set center alignment
  
  ps:`:` 's direction means the alignment.

  ---

### 9.Advanced skills

 #### supported HTML elements

 Those are not coverd in markdown marks, and can be directly write using HTML language.  

 So far,the supported HTML elements are:

 `<kbd>` defines keyboard word.It says the words are input from keyboard.
 `<b>` bold text.
 `<i>` italics text.
 `<em>` underlined.
 `<sup>` superscript.
 `<sub>` subscrept.
 `<br>` newLine.




