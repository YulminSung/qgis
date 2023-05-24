# qgis

## Python 주요 라이브러리

- geopandas 
 + 데이터프레임 + 지리공간데이터

- Shapely
 + 점, 선, 다각형(polygon) 2D 기하 도형 객체를 조작

- PyProj
 + 지리 좌표계와 투영 좌표계간 변환 (위도, 경도 변환)

- Rasterio
 + 위성이미지 저장, 불러오기, numpy 변환 등

## Raster vs Vector
- Raster Data
 + 셀 또는 픽셀 그리드 표현 (https://rfriend.tistory.com/589)
 + 위성 이미지, 항공사진 같은 시각화
 + 고도(Elevation, 온도)

- Vector Data
 + 점, 선, 다각형 특징을 좌표
 + 빌딩의 경계, 호수, 강 등 지구의 표면적인 특징 표현
 + 빌딩의 정보 주소, 가격, 건축날짜 등과 같은 정보를 **Polygon** 형태에 저장시킬 수 있음
 + Polygon - 각각의 좌표 및 성질 포함

## Shapefile
- 지리공간 벡터 데이터의 파일 형태
 + 세가지 파일 형태(.shp, .shx, .dbf) 로 구성
 + .shp : vector geometry 포함 (점, 선, 다각형)
 + .shx : 인덱스 파일, .shp 파일에 빠르게 접근할 수 있도록 도와주는 역할
 + .dbf : 각 vector feature들의 속성 정보들이 포함 
 + --> 이미지, 데이터 들이 포함되어 있어서 나누어 표현한다고 이해하기

## CRS (Coordinate Reference System)
- 좌표체계 : 위도, 경도

- 세가지 유형 : GCS, PCS, VCS
 + GCS(Geograpoc Coordinate systems) 
   + 위도 및 경도 좌표 (WGS84, NAD83)

 + PCS(Projected Coordinate systems)
   + 투영 좌표계 - 곡면을 표면으로 변환 (거리, 방향, 면적에 의해 왜곡이 발생할 수 있음)

 + VCS(Vertical Coordicate systems)
   + 해양과학 해수면과 관련

## Jupyter lab 실행
- git bash에 'jupyter lab' 입력 (가상환경 시스템에서)