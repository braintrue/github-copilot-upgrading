# upgraded 폴더 구조 설명

`upgraded` 폴더는 `legacy` 폴더의 전체 파일 및 디렉터리 구조를 그대로 복사한 디렉터리입니다. 각 구성 요소는 다음과 같습니다:

- `MANIFEST.in`: 패키징에 포함될 파일 목록을 지정하는 파일
- `README.rst`: 프로젝트 설명 파일
- `distribute-0.6.10.tar.gz`, `distribute_setup.py`: 배포 및 설치 관련 파일
- `setup.py`: Python 패키지의 설치 및 배포를 위한 설정 파일
- `docs/`: 프로젝트 문서 디렉터리
  - `build/`: 빌드된 문서(HTML, doctree 등)
  - `source/`: Sphinx 등으로 관리되는 문서 소스(rst, conf.py 등)
- `guachi/`: 주요 Python 패키지 소스 코드
  - `__init__.py`, `config.py`, `database.py`: 패키지 모듈
  - `tests/`: 테스트 코드
- `guachi.egg-info/`: 패키지 메타데이터 정보
  - `PKG-INFO`, `SOURCES.txt`, `dependency_links.txt`, `top_level.txt`

이 구조는 레거시 프로젝트의 전체 소스, 문서, 테스트, 패키징 정보를 포함하며, 업그레이드 작업의 출발점이 됩니다.