It has been mentioned that we understand the inner workings of the programming, so we would try to look at the python code
```
def two_sum(num,target):

        for i in range(0,len(num)):
        pointer_1=num[i]
        if pointer_1+num[i+1]==target:
        result=[i,i+1]
        return result
```
These are simplest line of codes, but if we try to replicate the same thing over Java, we would be getting `Array out of bounds` error, because when we do `num[i+1]`, we have got to take care of the fact that within the loop at the end, it's gonna go out of bounds for sure if we need to take care of that. In Python, we didn't need to take care for that because Python is basically a tool to solve complex problems not necesarily restricted to programming fundamental but a lot more. But in Java, we have to make sure to take care of the core programming concepts. Nevertheless, Java is strictly oops based. Finally the same code in Java is put at the bottom.

```
package LeetCode;

import java.util.Arrays;

public class Solution {
    public static void main(String[] args) {

        System.out.println(Arrays.toString(twoSum(new int[]{2, 7, 11, 15}, 9)));


    }

    public static int[] twoSum(int[] nums, int target) {
        int[] result = new int[2];

        for (int i = 0; i < nums.length; i++) {
            int pointer_1 = nums[i];
            if (i+1<=nums.length-1){
                if(pointer_1 + nums[i + 1] == target){
                    result = new int[]{i, i + 1};

                }
            }



        }

        return result;
    }
}
```
- output `[0, 1]`
- The leetcode problem can be seen here, `https://leetcode.com/problems/two-sum/`

Nevertheless, the solution needs to be fixed here because I was not checking the solution over LeetCode, here's the complete view.

![LeetCode](https://github.com/anindameister/RohanSingh/blob/main/photos/LeetCode/1.PNG) 

- Again, coming back to the point of discussion

![Why Java](https://github.com/anindameister/RohanSingh/blob/main/photos/Picture1.png) 

- There's a history of Java, which I don't think would be asked over the interview that I have tomorrow 19Jan2022, so am skipping the details and putting the slide.

![Introduction to Java](https://github.com/anindameister/RohanSingh/blob/main/photos/Picture2.png) 

- Java is object oriented `Java is an object-oriented programming language where every program has at least one class. Programs are often built from many classes and objects, which are the instances of a class.`
    - class: `A class is a user defined blueprint or prototype from which objects are created. It represents the set of properties or methods that are common to all objects of one type`
    - object: `An object is an instance of a class. A class is a template or blueprint from which objects are created. So, an object is the instance(result) of a class.`
- Java is Platform Independent: `This means that Java code can be run in any platform