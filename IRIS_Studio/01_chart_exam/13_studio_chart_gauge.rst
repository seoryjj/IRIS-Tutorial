Gauge
============================================================================

| 백분율 데이터를  Gauge 형태로 보여 줍니다. 



데이터 모델
------------------------------

| 데이터 모델 : EDU_SYSLOG_2020_0325_09
| 기간 : 2020/03/25 09:00 ~ 10:00
| 내용 : 서버(HOST) 에서 출력되는 SYSLOG 데이터
|

.. list-table::
   :header-rows: 1

   * - DATETIME
     - HOST
     - FACILITY
     - PRIORITY
     - LEVEL
     - LEVEL_INT
     - TAG
     - PROGRAM
   * - 20200325090401
     - tsdn-svr1
     - cron
     - info
     - info
     - 7
     - 4e
     - CROND
   * - 20200325090401
     - gcs1
     - daemon
     - info
     - info
     - 7
     - 1e
     - systemd
   * - ...
     - ...
     - ...
     - ...
     - ...
     - ...
     - ...
     - ...    
   * - 20200325100424
     - tsdn-svr1
     - kern
     - warning
     - warning
     - 5
     - 04
     - kernel





Gauge 챠트
-------------------------------------------

- 검색어


.. code::

  * | where HOST='tsdn-svr1' 
    | sql "select round(count(*) / 37940 * 100, 2)  from angora"


| SYSLOG 데이터중 HOST = 'tsdn-svr1'  를 대상으로
| 전체 SYSLOG row count 인  37940 대비 HOST = 'tsdn-svr1' 의 row count 의 비율을 구하는 검색어입니다.
| 현재 Gauge chart 는 백분율에 단일 값만 그려집니다.(=> 추후에 normal, minor, major, critical 같은 라벨의 범위를 표시할 수 있게 개선할 예정입니다.)
|


.. image:: images/chart_gauge_25.png
    :alt: chart_gauge_25


| 시각화옵션에서 글꼴과 글자크기, 색상, 스타일, 정렬 등을 지정할 수 있습니다.
