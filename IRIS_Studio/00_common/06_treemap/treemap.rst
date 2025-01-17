===================================================================
트리맵
===================================================================
| 참고 보고서 : 
| `템플릿_EDU_Studio treemap chart_데이터객체버전 <http://b-iris.mobigen.com:80/studio/exported/0336c604d0ce4fbb98e283484888c84b62ba0a7693e34629bbdb290a1adba218>`__ 
|
데이터를 그룹과 그 그룹의 값에 따라 크기와 색을 다르게 표현하는 트리맵을 보고서에 추가하는 방법에 관하여 기술합니다.

| 
.. contents::
    :backlinks: top
    
| 
-------------------------------------------------------------------
트리맵 차트 영역 생성
-------------------------------------------------------------------
- 표시된 "차트" 아이콘을 클릭한 후 마우스 드래그 앤 드롭으로 테이블이 그려질 영역을 생성합니다.

.. image:: ./images/tu_01.png
    :alt: 트리맵_차트영역생성

| 
-------------------------------------------------------------------
데이터 설정
-------------------------------------------------------------------
- 우측의 "데이터" 탭에서 자동추가를 클릭 후 데이터 모델 객체에서 가져올 데이터 모델을 선택해줍니다.
- 그리고 싶은 차트에 맞게 검색어를 써서 원하는 차트를 출력할 수 있습니다.
- 또한, 연결하고 싶은 데이터 모델 객체가 따로 있었다면 설정을 자동추가를 클릭하는 대신 밑에 설정을 클릭하고 원하는 데이터 모델 객체를 선택해주면 됩니다.

.. image:: ./images/tree_04.png
    :alt: 트리맵_데이터설정
| 
-------------------------------------------------------------------
시각화 옵션 설정
-------------------------------------------------------------------
- 원하는 테이블로 나왔는지 확인한 후 우측 "시각화" 탭에서 시각화 유형을 트리맵으로 선택해줍니다.
- 차트 화면을 우클릭 하면 그리고자 하는 차트에 맞게 시각화 옵션으로 세부적인 것들을  조정할 수 있습니다.

.. image:: ./images/tree_05.png
    :alt: 트리맵_시각화 옵션 설정


시각화 옵션
=================================================================

.. |opt1| image:: ./images/tree_01.PNG
    :scale: 90%
    :alt: 트리맵 시각화 옵션 (1) - 일반

.. |opt2| image:: ./images/tree_02.PNG
    :scale: 90%
    :alt: 트리맵 시각화 옵션 (2) - 범례

.. |opt3| image:: ./images/tree_03.PNG
    :scale: 90%
    :alt: 트리맵 시각화 옵션 (3) - 데이터


.. list-table::
   :header-rows: 1

   * - 옵션
     - 설명
   * - |opt1|
     - 데이터 값의 표현여부, 배경색상, 다운로드 및 상세보기 버튼 설정
   * - |opt2|
     - 트리맵에 표시되는 범례의 여부를 설정
   * - |opt3|
     - 트리맵에 표시되는 데이터의 그룹 및 값을 설정. 최초의 실행(Run) 후에 변경 가능
     
| 
시각화 옵션 예시
=================================================================
- 데이터 선택을 안하면 아래와 같이 색상 차이만 보실 수 있습니다.
- 또한 최소값과 최대값 색상을 데이터 값에 맞게 원하는 색상으로 나타내실 수 있습니다.
.. image:: ./images/tree_07.png
    :alt: 트리맵_시각화 결과 확인

| 
-------------------------------------------------------------------
결과 확인
-------------------------------------------------------------------
- 설정을 마친 후 우측 하단의 실행 버튼을 클릭하면, 아래 그림과 같이 결과가 표시됩니다.
- 제대로 적용됐는지 확인하고자 한다면, 우측 상단의 보기 버튼을 눌러 작성 결과를 다시 한 번 확인하면 됩니다.
- 결과가 정상적으로 표출될 경우, 작성 화면에서 빠른저장 버튼을 눌러 결과를 저장합니다.
- 자동저장이 안되기 때문에 수시로 빠른 저장을 눌러줘야 합니다.


.. image:: ./images/tree_06.png
    :alt: 트리맵_시각화 결과 확인

| 
-------------------------------------------------------------------
주의사항
-------------------------------------------------------------------

.. code::

    보기 버튼을 눌렀을 때, 차트가 자동으로 실행되지 않을 경우,

    "자동 실행"을 설정하지 않을 경우 보고서 조회 시 자동으로 실행되지 않습니다.

    데이터 탭 하단의 데이터 실행방법 설정에 있는 "자동 실행"을 선택한 후 다시 확인해보시기 바랍니다.
    (아래 그림 참조)

.. image:: ./images/tu_02.png
    :scale: 90%
    :alt: 자동실행 설정

.. code::

    차트에 아무 컬럼도 표시되지 않을 경우,

    1) 시각화 옵션 데이터 설정에 오류가 있는지 확인합니다.
    2) 데이터 설정에 문제가 없다면, 우측 하단의 실행 버튼을 클릭한 후 다시 확인하시기 바랍니다.


