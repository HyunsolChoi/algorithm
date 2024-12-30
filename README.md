

## �Ұ� �� ����

**Crime Data Sorting Program**
2018 ~ 2022���� ��ī�� ���� �����͸� ������� ��, ��, ���� ������ ���� �� Attribute�� ���� ������ �����ϰ�,
����ڿ��� ���ĵ� �����͸� �����ϴ� ���α׷��Դϴ�.

����� ���� ����� �Ϻθ� �켱 �����Ͽ� ������ �Ϸ�Ǿ����� ����ڿ��� Ȯ�ν�Ű��,
������ �� ��ü �����ʹ� ������ csv ���Ϸ� �����մϴ�. 

�� ��ܿ��� ���α׷��� �ε� �ÿ� data1.csv data2.csv�� �о� �� ������ ���� ���� ����մϴ�.

�߾ӿ��� ���ĵ� ������ csv ������ ���� ������ ���� �ش� ������ ���� ��ư�� �����ݴϴ�.

�������� Ư�� Key������ ���� ��, �� �˰��� �� �ҿ�ð��� ����մϴ�.
(���� 10ȸ �ݺ��� ��쿡�� �ð��� �����Ͽ� ������ 10�� �� �ð��� ���)

2�࿡ ��ġ�� 5���� ��ư�� ���Ŀ� ����� Key�� �����ϴ� ��ư�̸� ���� �� ������ ����Ǹ� �ε� ȭ���� ��µ˴ϴ�.

��ư�� ���� üũ�ڽ��� 10ȸ �ݺ� ���θ� Ȯ���մϴ�.
10ȸ �ݺ� �� ��� �ð��� ����Ͽ� ���� ��Ȯ�� ���� �ð��� Ȯ�� ����������, �ҿ� �ð��� ��ϴ�.
(�ʹ� �÷��ɸ��� ���� ����� 100ȸ, 1000ȸ�� �ƴ� 10ȸ�� ����)

�ϴ��� DataGrid�� ���ĵ� �������� �Ϻθ� ���� ��ȣ(index)�� �Բ� ����մϴ�.
*���� ���� �߿��� �ε� ȭ������ ��ü�˴ϴ�.**

## ���� / ���� ����

 - Data ���� ���� data1.csv data2.csv ������ ���Ƿ� �̸��� *����*, *����*�ϸ� ���α׷��� ���������� ���ư��� ���� �� �ֽ��ϴ�.

 - ������ ������ �Ϸ�Ǹ� Data ������ SortedData1.csv SortedData2.csv �� �����˴ϴ�. 
   �̴� ������ �Ϸ�� �����ͷ�, csv�� �ִ� ���� ���� ����Ͽ� �� �ݾ� �����͸� �����Ͽ����ϴ�.

 - ����� �˰����� �ڵ�� Models�� SortAlgorithms.cs�� �ۼ��Ǿ� �ֽ��ϴ�.


 # Add eng version for encoding error

 ## Introduction and Usage

**Crime Data Sorting Program**
This program is designed to sort Chicago crime data from 2018 to 2022 
using Quick, Heap, and Merge sorting algorithms based on different attributes, providing users with the sorted data.

The program initially provides a portion of the sorted results to confirm to the user that the sorting has been completed, 
and the entire sorted dataset is provided in a separate CSV file.

The top left displays the total number of rows loaded from `data1.csv` and `data2.csv` when the program loads.

The center of the interface shows a button to open the sorted CSV file if it exists.

The right side displays the sorting times for each algorithm when sorted by a specific key. 
If the sorting is repeated 10 times, the average time is displayed (total time divided by 10).

In the second row, there are 5 buttons to specify the sorting key. When clicked, sorting is performed, and a loading screen is displayed.

The checkbox to the right of the buttons determines whether to repeat the sorting 10 times. 
Sorting 10 times provides a more accurate average sorting time but takes longer. 
(To prevent excessively long wait times, the number of repetitions is set to 10 rather than 100 or 1000.)

The `DataGrid` at the bottom displays part of the sorted data, along with the row index. *During sorting, the loading screen is displayed.*

## Notes / Important Information

 - The `data1.csv` and `data2.csv` files in the `Data` folder should not be *renamed* or *deleted*, as this may prevent the program from functioning correctly.

 - Once sorting is complete, `SortedData1.csv` and `SortedData2.csv` are created in the `Data` folder. These files contain the sorted data, split in half to accommodate the maximum number of rows per CSV file.

 - The code for the sorting algorithms used is written in `SortAlgorithms.cs` under the `Models` directory.

