# Algorithm

## #1

twoSum함수에 숫자배열과 '특정 수'를 인자로 넘기면,
더해서 '특정 수'가 나오는 index를 배열에 담아 return해 주세요.

nums: 숫자 배열
target: 두 수를 더해서 나올 수 있는 합계
return: 두 수의 index를 가진 숫자 배열
예를 들어,
nums은 [4, 9, 11, 14]
target은 13

nums[0] + nums[1] = 4 + 9 = 13 이죠?

그러면 [0, 1]이 return 되어야 합니다.

가정
target으로 보내는 합계의 조합은 배열 전체 중에 2개 밖에 없다고 가정하겠습니다.

<br>
<br>

```jsx

nums = [1,3,5,7,9];
target = 8;
let index = [];

function twoSum(array, num) {
    
    for (let i = 0; i < array.length; i++) {
      for (let i = 0; j < array.length; i++) {
        if (array[i] + array[j] === target){
            index.push(i,j);
        }
     }
 }
return index;
}
twoSum(nums, target); 

```

<br>

## 🌐풀이과정 

처음 접근은 `숫자배열`과 `특정 수`를 인자로 넘긴다는 것을 생각하고 변수를 정해줬다. <br>
숫자배열 `nums` 의 두 수를 더할때 `target` 이라는 합계가 나온다. <br>
배열의 두 수를 구하기 위해 인자 `array`의 `length` 길이만큼 for문을 **두 번**  돌려주고 <br>
if문에서 `array의 인덱스` 를 더했을 때 target과 같다면 빈 리스트 `index` 에 push를 한다



