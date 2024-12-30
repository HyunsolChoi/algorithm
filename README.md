

## 소개 및 사용법

**Crime Data Sorting Program**
2018 ~ 2022년의 시카고 범죄 데이터를 기반으로 퀵, 힙, 병합 정렬을 통해 각 Attribute에 따른 정렬을 수행하고,
사용자에게 정렬된 데이터를 제공하는 프로그램입니다.

수행된 정렬 결과의 일부를 우선 제공하여 정렬이 완료되었음을 사용자에게 확인시키고,
정렬이 된 전체 데이터는 별개의 csv 파일로 제공합니다. 

좌 상단에는 프로그램이 로드 시에 data1.csv data2.csv를 읽어 총 데이터 행의 수를 출력합니다.

중앙에는 정렬된 데이터 csv 파일의 존재 유무에 따라 해당 파일을 여는 버튼을 보여줍니다.

우측에는 특정 Key값으로 정렬 시, 각 알고리즘 별 소요시간을 출력합니다.
(만일 10회 반복된 경우에는 시간을 총합하여 나누기 10을 한 시간을 출력)

2행에 위치한 5개의 버튼은 정렬에 사용할 Key를 지정하는 버튼이며 누를 시 정렬이 수행되며 로딩 화면이 출력됩니다.

버튼의 우측 체크박스는 10회 반복 여부를 확인합니다.
10회 반복 시 평균 시간을 출력하여 보다 정확한 정렬 시간을 확인 가능하지만, 소요 시간이 깁니다.
(너무 올래걸리는 것을 대비해 100회, 1000회가 아닌 10회로 지정)

하단의 DataGrid는 정렬된 데이터의 일부를 행의 번호(index)와 함께 출력합니다.
*정렬 수행 중에는 로딩 화면으로 대체됩니다.**

## 주의 / 참고 사항

 - Data 폴더 내의 data1.csv data2.csv 파일은 임의로 이름을 *변경*, *삭제*하면 프로그램이 정상적으로 돌아가지 않을 수 있습니다.

 - 데이터 정렬이 완료되면 Data 폴더에 SortedData1.csv SortedData2.csv 가 생성됩니다. 
   이는 정렬이 완료된 데이터로, csv의 최대 행의 수를 고려하여 반 반씩 데이터를 저장하였습니다.

 - 사용한 알고리즘의 코드는 Models의 SortAlgorithms.cs에 작성되어 있습니다.


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

