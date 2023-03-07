# bubble-sort
# 설명
서로간의 두가지 항목을 선택하여 비교해보고 큰것을 앞으로 이동시킨다.
# 예제
![img1 daumcdn](https://user-images.githubusercontent.com/126844596/223418934-3a6fe89f-2ecd-454b-b142-999c3072ffc5.gif)
# 자바
import java.util.Arrays;

public class bubbleSort {
public static void main(String[] args) {

int[] a = { 3, 5, 1, 2, 4 };

int tempValue;

for (int i = 0; i < a.length; i++) {

for (int j = 0; j < a.length - i - 1; j++) { // 0 ~ n, 0 ~ n-1 번 반복를 돌면서 바로 옆 숫자릴 비교

if (a[j] > a[j + 1]) {  // 바로 오른쪽 숫자와 비교하여 크기가 클 경우, 서로 위치를 바꿈

tempValue = a[j];

a[j] = a[j + 1];

a[j + 1] = tempValue;

				}
			}
		}
	System.out.println(Arrays.toString(a));
	}
}
