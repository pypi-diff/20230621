# Comparing `tmp/WebtoonScraper-0.1.0a1.tar.gz` & `tmp/WebtoonScraper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-0.1.0a1.tar", last modified: Mon Jun 19 03:52:40 2023, max compression
+gzip compressed data, was "WebtoonScraper-0.1.1.tar", last modified: Wed Jun 21 12:03:58 2023, max compression
```

## Comparing `WebtoonScraper-0.1.0a1.tar` & `WebtoonScraper-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:52:40.428008 WebtoonScraper-0.1.0a1/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.1.0a1/LICENSE
--rw-rw-rw-   0        0        0      140 2023-06-06 01:23:54.000000 WebtoonScraper-0.1.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0     6658 2023-06-19 03:52:40.428008 WebtoonScraper-0.1.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     5646 2023-06-18 13:17:35.000000 WebtoonScraper-0.1.0a1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:52:40.413076 WebtoonScraper-0.1.0a1/WebtoonScraper/
--rw-rw-rw-   0        0        0      516 2023-06-06 00:42:00.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/BestChallengeScraper.py
--rw-rw-rw-   0        0        0     6142 2023-06-19 03:38:04.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/BufftoonScraper.py
--rw-rw-rw-   0        0        0     3332 2023-06-07 11:43:11.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/NaverWebtoonScraper.py
--rw-rw-rw-   0        0        0    16541 2023-06-18 19:19:13.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/Scraper.py
--rw-rw-rw-   0        0        0     4665 2023-06-17 13:02:43.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/TelescopeScraper.py
--rw-rw-rw-   0        0        0     3438 2023-06-18 16:33:27.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/Webtoon.py
--rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/WebtoonCanvasScraper.py
--rw-rw-rw-   0        0        0     4250 2023-06-17 07:29:55.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/WebtoonOriginalsScraper.py
--rw-rw-rw-   0        0        0      568 2023-06-18 16:21:17.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/__init__.py
--rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.1.0a1/WebtoonScraper/foldermanagement.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:52:40.425804 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0     6658 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       29 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-19 03:52:40.000000 WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    29088 2023-06-06 01:18:53.000000 WebtoonScraper-0.1.0a1/number_from_manhwakyung.png
--rw-rw-rw-   0        0        0       42 2023-06-19 03:52:40.429009 WebtoonScraper-0.1.0a1/setup.cfg
--rw-rw-rw-   0        0        0     1862 2023-06-19 03:52:38.000000 WebtoonScraper-0.1.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:52:40.426998 WebtoonScraper-0.1.0a1/test/
--rw-rw-rw-   0        0        0      131 2023-06-18 16:21:20.000000 WebtoonScraper-0.1.0a1/test/test.py
--rw-rw-rw-   0        0        0   182776 2023-05-29 08:43:24.000000 WebtoonScraper-0.1.0a1/title_no_from_webtoons.com.png
--rw-rw-rw-   0        0        0    52914 2023-05-15 00:27:14.000000 WebtoonScraper-0.1.0a1/titleid_from_nw.png
+drwxrwxrwx   0        0        0        0 2023-06-21 12:03:58.127315 WebtoonScraper-0.1.1/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      140 2023-06-06 01:23:54.000000 WebtoonScraper-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10314 2023-06-21 12:03:58.126316 WebtoonScraper-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9226 2023-06-21 11:54:52.000000 WebtoonScraper-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 12:03:58.108159 WebtoonScraper-0.1.1/WebtoonScraper/
+-rw-rw-rw-   0        0        0      516 2023-06-06 00:42:00.000000 WebtoonScraper-0.1.1/WebtoonScraper/BestChallengeScraper.py
+-rw-rw-rw-   0        0        0     6198 2023-06-21 11:41:23.000000 WebtoonScraper-0.1.1/WebtoonScraper/BufftoonScraper.py
+-rw-rw-rw-   0        0        0     7405 2023-06-21 11:54:44.000000 WebtoonScraper-0.1.1/WebtoonScraper/NaverPostScraper.py
+-rw-rw-rw-   0        0        0     3332 2023-06-07 11:43:11.000000 WebtoonScraper-0.1.1/WebtoonScraper/NaverWebtoonScraper.py
+-rw-rw-rw-   0        0        0    16642 2023-06-21 08:37:42.000000 WebtoonScraper-0.1.1/WebtoonScraper/Scraper.py
+-rw-rw-rw-   0        0        0     4665 2023-06-17 13:02:43.000000 WebtoonScraper-0.1.1/WebtoonScraper/TelescopeScraper.py
+-rw-rw-rw-   0        0        0     4284 2023-06-21 12:03:29.000000 WebtoonScraper-0.1.1/WebtoonScraper/Webtoon.py
+-rw-rw-rw-   0        0        0      501 2023-06-06 00:44:55.000000 WebtoonScraper-0.1.1/WebtoonScraper/WebtoonCanvasScraper.py
+-rw-rw-rw-   0        0        0     4250 2023-06-17 07:29:55.000000 WebtoonScraper-0.1.1/WebtoonScraper/WebtoonOriginalsScraper.py
+-rw-rw-rw-   0        0        0      630 2023-06-21 11:25:23.000000 WebtoonScraper-0.1.1/WebtoonScraper/__init__.py
+-rw-rw-rw-   0        0        0     9473 2023-05-17 13:49:27.000000 WebtoonScraper-0.1.1/WebtoonScraper/foldermanagement.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:03:58.124313 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0    10314 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 12:03:58.000000 WebtoonScraper-0.1.1/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 12:03:58.127315 WebtoonScraper-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1879 2023-06-21 11:51:34.000000 WebtoonScraper-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 12:03:58.125316 WebtoonScraper-0.1.1/test/
+-rw-rw-rw-   0        0        0      308 2023-06-21 12:02:19.000000 WebtoonScraper-0.1.1/test/test.py
```

### Comparing `WebtoonScraper-0.1.0a1/LICENSE` & `WebtoonScraper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0a1/PKG-INFO` & `WebtoonScraper-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: WebtoonScraper
-Version: 0.1.0a1
-Summary: Scraping webtoons and some utils for it
-Home-page: https://github.com/ilotoki0804/WebtoonScraper
-Author: ilotoki0804
-Author-email: ilotoki0804@gmail.com
-License: MIT
-Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
 
 # 시작하기
 
 1. 파이썬을 설치합니다.
@@ -31,52 +13,103 @@
 
    또는
 
    ```
    pip3 install -U WebtoonScraper
    ```
 
-# 웹툰 다운로드하기
-
+# 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경 다운로드하기
+버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/titleid_from_nw.png)
+   ![img](naver_webtoon.png)
    국내의 경우 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/title_no_from_webtoons.com.png)
+   ![img](webtoons_original.png)
    해외의 경우는 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/number_from_manhwakyung.png)
+   ![img](manhwakyung.png)
    만화경의 경우는 여기에서 확인할 수 있습니다.
-2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스 모두 가능합니다.
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
    wt.get_webtoon(76648, wt.N) # titleid를 여기에다 붙여넣으세요.
    # 베스트 도전만화
    wt.get_webtoon(763952, wt.B) # titleid를 여기에다 붙여넣으세요.
-   # 해외 웹툰 오리지널
+   # 웹툰 오리지널
    wt.get_webtoon(1435, wt.O) # titleid를 여기에다 붙여넣으세요.
-   # 해외 웹툰 캔버스
+   # 웹툰 캔버스
    wt.get_webtoon(304446, wt.C) # titleid를 여기에다 붙여넣으세요.
    # 만화경
    wt.get_webtoon(146, wt.M) # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
    cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 하지만 이 방식은 서로 다른 사이트에서 id가 겹치는 웹툰이 존재하면 오작동할 수 있으니 꼭 태그를 붙이는 것을 추천합니다.
 
-   또 merge 태그를 이용하면
+   또 merge 태그를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 자동으로 5화씩 묶습니다.
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 중간에 웹툰 다운로드가 멈춘 듯이 보여도 정상입니다. 그대로 가만히 있으면 다운로드가 다시 진행됩니다.
 * 만약 작동하지 않는다면 윈도우에서 Python 3.11.3을 설치하고 앞의 과정을 반복해 보세요.
 
+# 버프툰 다운로드하기
+## 로그인하지 않은 상태에서 웹툰 다운로드하기(추천하지 않음)
+로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+
+   wt.get_webtoon(1007888, wt.BU) # 복사했던 숫자를 여기에다 붙여넣으세요.
+   ```
+3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
+4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
+## 로그인한 상태에서 웹툰 다운로드하기
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
+2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 아무 웹툰이나 들어갑니다.
+3. 아무 요청이나 클릭하고 나온 창에 '머리글' 탭을 엽니다.
+4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
+5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+
+   wt.get_webtoon(1007888, wt.BU) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   ```
+6. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
+4. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+# 네이버 포스트 다운로드하기
+
+1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
+   ![img](naver_post.png)
+<!-- 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+
+   wt.get_post(597061, 19803452) # seriesNo와 memberNo를 차례대로 입력해주세요.
+   ``` -->
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+
+   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   ```
+3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
+   ```
+   Enter memberNo 19803452
+   ...진행됨...
+   ```
+4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
+## 주의사항
+* get_webtoon이 **아닌** get_post 함수를 사용한다는 점을 주의하세요.
+* 웹툰 태그(Webtoon.P)를 작성할 필요가 없으며 작성하면 오류가 난다는 점을 주의하세요.
+* 가끔씩 이유 없는 오류가 발생할 수 있습니다. 
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import *
 
@@ -113,14 +146,22 @@
 
 ### ID를 회차 번호로 그대로 사용하는 이유
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
-## 전 버전과의 차이
+# Relese Note
+
+0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
+
+0.1.0: 버프툰 추가, 빠진 부분 재추가
 
 0.0.19.3: merge 속성 추가, get_webtoon 함수로 변경
+
 0.0.19.1: pbar에 표시되는 내용 변경, 내부적 개선
+
 0.0.18: 만화경 지원, 리팩토링됨(Scraper Abstract Base Class 추가)
+
 0.0.17: 웹툰즈 오리지널, 캔버스 지원
+
 0.0.12: 네이버 웹툰, 베스트 도전 지원
```

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/BestChallengeScraper.py` & `WebtoonScraper-0.1.1/WebtoonScraper/BestChallengeScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/BufftoonScraper.py` & `WebtoonScraper-0.1.1/WebtoonScraper/BufftoonScraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 '''Download Webtoons from Bufftoon.
 '''
 import re
 from pathlib import Path
 import time
 from async_lru import alru_cache
 from WebtoonScraper.Scraper import Scraper
+
 class BufftoonScraper(Scraper):
     '''Scrape webtoons from Naver Webtoon.'''
-    def __init__(self, pbar_independent=False, short_connection=False, cookie=None):
+    def __init__(self, pbar_independent=False, short_connection=False, cookie: str=''):
         super().__init__(pbar_independent, short_connection)
         self.BASE_URL = 'https://bufftoon.plaync.com'
         if not short_connection:
             self.IS_STABLE_CONNECTION = True
         self.COOKIE = cookie
     
     @alru_cache(maxsize=4)
@@ -22,20 +23,20 @@
         # print(raw_data)
         subtitles = {}
         episode_ids = {}
         for raw_episode in raw_data['result']['episodes']:
             if not get_payment and raw_episode['isPaymentEpisode']:
                 if self.PBAR_INDEPENDENT:
                     pass
-                print(f"Episode '{raw_episode['title']}' is not free of charge episode")
+                print(f"Episode '{raw_episode['title']}' is not free of charge episode. It'll be not downloaded.")
                 continue
             if not self.COOKIE and not raw_episode['isOpenFreeEpisode']:
                 if self.PBAR_INDEPENDENT:
                     pass
-                print(f"Episode '{raw_episode['title']}' is not opened for non-login users.")
+                print(f"Episode '{raw_episode['title']}' is not opened for non-login users. It'll be not downloaded.")
                 continue
             episode_no = raw_episode['episodeOrder']
             raw_episode_id = raw_episode['listImgPath']
             # print(raw_episode_id)
             episode_id = int(re.search(rf'(?<=contents\/.\/{titleid}\/)(\d+)(?=\/)', raw_episode_id).group(0))
             episode_ids[episode_no] = episode_id
             subtitles[episode_no] = raw_episode['title']
```

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/NaverWebtoonScraper.py` & `WebtoonScraper-0.1.1/WebtoonScraper/NaverWebtoonScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/Scraper.py` & `WebtoonScraper-0.1.1/WebtoonScraper/Scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,24 +165,25 @@
 
         Args:
             filename_or_url: 파일 확장자가 궁금한 파일명이나 URL. 이때 URL 쿼리는 무시됩니다.
         
         Returns:
             파일 확장자를 반환합니다.
         """
-        return re.search(r'(?<=[.])(jpg|png|jpeg|gif)(?=[?].+$|$)', filename_or_url, re.I).group()
+        serch_result: re.Match = re.search(r'(?<=[.])(jpg|png|jpeg|gif)(?=[?].+$|$)', filename_or_url, re.I)
+        return serch_result.group()
         # return filename_or_url.split('.')[-1].lower()
 
     @staticmethod
     def get_acceptable_file_name(file_or_diretory_name: str, strict_checking: bool=False) -> str:
         """Translate file or diretory name to accaptable name.
 
         Caution: Don't put here diretory path beacause it will translate slash and backslash to acceptable(and cannot be used for going directory) name.
         """
-        table = str.maketrans('\\/:*?"<>|\t', '⧵／：＊？＂＜＞∣  ')
+        table = str.maketrans('\\/:*?"<>|\t\n', '⧵／：＊？＂＜＞∣   ')
 
         processed = html.unescape(file_or_diretory_name) # change things like "&amp;" to "'".
         
         processed = processed.translate(table).strip()
 
         processed = re.sub(r'\.$', '．', processed)
 
@@ -193,15 +194,15 @@
                                      22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 34, 42, 58, 60, 62, 63, 124):
                     strict_checked_string += ' '
                 else:
                     strict_checked_string += chractor
             return strict_checked_string
         return processed
     
-    def set_folders(self, base_dir: str='Python/files/webtoon') -> str:
+    def set_folders(self, base_dir: str='Python/files/webtoon') -> None:
         """Set base folder."""
         self.BASE_DIR = Path(base_dir)
 
 ################################## MAIN ACTION ##################################
 
     def download_one_webtoon(self, titleid: int, value_range: tuple|int|None=None) -> None:
         """async를 사용하지 않는 일반 상태일 경우 사용하는 함수이다. 사용법은 download_one_webtoon_async와 동일하다."""
@@ -255,31 +256,31 @@
     
     @abstractmethod
     async def get_all_episode_no(self, titleid: int, attempt: int) -> Iterable:
         """웹툰에서 전체 에피소드를 가져온다."""
         pass
 
     # @profile
-    def _check_validate_of_files(self, episode_dir: Path, episode_no: int, image_urls: list) -> None|bool:
+    def _check_validate_of_files(self, episode_dir: Path, episode_no: int, image_urls: list, subtitle: str) -> None|bool:
         """episode_dir를 생성하고 이미 있다면 해당 폴더 내 내용물이 적합한지 조사한다.
 
         None를 return한다면 회차를 다운로드해야 한다는 의미이다.
         True를 return하면 해당 회차가 이미 완전히 다운로드되어 있으며, 따라서 다운로드를 지속할 이유가 없음을 의미한다.
         """
         try:
             episode_dir.mkdir()
         except FileExistsError:
-            self._set_pbar(f'checking integrity of {episode_no=}')
+            self._set_pbar(f'checking integrity of {subtitle}')
             is_filename_appropriate = all(re.match(r"\d{3}[.](png|jpg|jpeg|bmp|gif)", file) for file in os.listdir(episode_dir))
             if not is_filename_appropriate or not len(image_urls) == len(os.listdir(episode_dir)):
-                self._set_pbar(f'{episode_no=} is not vaild. Automatically restore files.')
+                self._set_pbar(f'{subtitle} is not vaild. Automatically restore files.')
                 shutil.rmtree(episode_dir)
                 episode_dir.mkdir()
             else:
-                self._set_pbar(f'skipping {episode_no=}')
+                self._set_pbar(f'skipping {subtitle}')
                 return True
 
     # @profile
     async def download_one_episode(self, episode_no: int, titleid: int, webtoon_dir: Path) -> None:
         """한 회차를 다운로드받는다."""
         subtitle = await self.get_subtitle(titleid, episode_no, file_acceptable=True)
 
@@ -287,18 +288,18 @@
             print(f'this episode is not free or not yet created. This episode won\'t be loaded. {episode_no=}')
             self._set_pbar('unknown episode')
             return
 
         episode_images_url = await self.get_episode_images_url(titleid, episode_no)
 
         episode_dir = webtoon_dir / f'{episode_no:04d}. {subtitle}'
-        if self._check_validate_of_files(episode_dir, episode_no, episode_images_url):
+        if self._check_validate_of_files(episode_dir, episode_no, episode_images_url, subtitle):
             return
 
-        self._set_pbar('downloading')
+        self._set_pbar(f'downloading {subtitle}')
         get_image_coroutines = (self.download_single_image(episode_dir, element, i) for i, element in enumerate(episode_images_url))
         await asyncio.gather(*get_image_coroutines)
 
     @abstractmethod
     async def get_subtitle(self, titleid: int, episode_no: int, file_acceptable: bool) -> str:
         """부제목, 즉 회차의 제목을 불러온다."""
         pass
@@ -307,14 +308,15 @@
     async def get_episode_images_url(self, titleid: int, episode_no: int) -> list:
         """해당 회차를 구성하는 이미지들을 불러온다."""
         pass
 
     # @profile
     async def download_single_image(self, episode_dir: Path, url: str, image_no: int) -> None:
         """Download image from url and returns to {episode_dir}/{file_name(translated to accactable name)}."""
+        # print(url)
         image_extension = self.get_file_extension(url)
         file_name = f'{image_no:03d}.{image_extension}'
 
         # self._set_pbar(f'{episode_dir}|{file_name}')
         image_raw = await self.get_internet(get_type='requests', url=url, is_run_in_executor=True)
         image_raw = image_raw.content
```

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/TelescopeScraper.py` & `WebtoonScraper-0.1.1/WebtoonScraper/TelescopeScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/Webtoon.py` & `WebtoonScraper-0.1.1/WebtoonScraper/Webtoon.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 
 from WebtoonScraper.NaverWebtoonScraper import NaverWebtoonScraper
 from WebtoonScraper.foldermanagement import WebtoonFolderManagement
 from WebtoonScraper.WebtoonOriginalsScraper import WebtoonOriginalsScraper
 from WebtoonScraper.BestChallengeScraper import BestChallengeScraper
 from WebtoonScraper.WebtoonCanvasScraper import WebtoonCanvasScraper
 from WebtoonScraper.TelescopeScraper import TelescopeScraper
-from WebtoonScraper.BufftoonScraper import BufftoonScraper
+from WebtoonScraper.BufftoonScraper import BufftoonScraper 
+from WebtoonScraper.NaverPostScraper import NaverPostScraper 
 
 N = NAVER_WEBTOON = 'naver_webtoon'
 B = BEST_CHALLENGE = 'best_challenge'
 O = ORIGINALS = 'originals'
 C = CANVAS = 'canvas'
 T = M = TELESCOPE = 'telescope'
 BU = BT = BUFFTOON = 'bufftoon'
+P = POST = NAVER_POST = 'naver_post'
 
 async def auto_webtoon_type(webtoon_id: int) -> str:
     """If webtoon is best challenge, this returns True. Otherwise, False."""
     webtoonscraper = NaverWebtoonScraper()
 
     title = await webtoonscraper.get_internet('soup_select_one', f'https://comic.naver.com/webtoon/detail?titleId={webtoon_id}', 'meta[property="og:title"]')
     title = title.get('content')
@@ -53,26 +55,38 @@
         webtoonscraper = WebtoonOriginalsScraper()
     elif webtoon_type.lower() == CANVAS:
         webtoonscraper = WebtoonCanvasScraper()
     elif webtoon_type.lower() == TELESCOPE:
         webtoonscraper = TelescopeScraper()
     elif webtoon_type.lower() == BUFFTOON:
         webtoonscraper = BufftoonScraper()
+    elif webtoon_type.lower() == NAVER_POST:
+        webtoonscraper = NaverPostScraper()
     else:
         raise ValueError('webtoon_type should be among naver_webtoon, best_challenge, originals, canvas, and telescope.')
     return webtoonscraper
 
-async def get_webtoon_async(webtoon_id:int, webtoon_type:str=None, merge:None|int=None) -> None:
+async def get_webtoon_async(webtoon_id:int, webtoon_type:str=None, *, merge:None|int=None, cookie: None|str=None, member_no: None|int=None) -> None:
     if webtoon_type is None:
         webtoon_type = await auto_webtoon_type(webtoon_id)
     webtoonscraper = await get_webtoon_type(webtoon_type)
-    await webtoonscraper.download_one_webtoon_async(titleid=webtoon_id)
+    if webtoon_type.lower() == BUFFTOON:
+        if cookie is None:
+            webtoonscraper.COOKIE = cookie
+        else:
+            webtoonscraper.COOKIE = input(f'Enter cookie of {webtoon_id} (Enter nothing to preceed without cookie)')
+    if webtoon_type.lower() == NAVER_POST:
+        if not member_no:
+            member_no = int(input(f'Enter memberNo of {webtoon_id}'))
+        await webtoonscraper.download_one_webtoon_async(titleid=webtoon_id, member_no=member_no)
+    else:
+        await webtoonscraper.download_one_webtoon_async(titleid=webtoon_id)
     if merge:
         fd = WebtoonFolderManagement('webtoon_merge')
         fd.divide_all_webtoons(merge)
 
-def get_webtoon(webtoon_id:int, webtoon_type:str=None, merge:None|int=None) -> None:
-    asyncio.run(get_webtoon_async(webtoon_id, webtoon_type, merge))
+def get_webtoon(webtoon_id:int, webtoon_type:str=None, *, merge:None|int|bool=None, cookie: None|str=None, member_no: None|int=None) -> None:
+    asyncio.run(get_webtoon_async(webtoon_id, webtoon_type, merge=merge, cookie=cookie, member_no=member_no))
 
 if __name__ == '__main__':
-    # get_webtoon(263735)
-    get_webtoon(263735, merge=True)
+    get_webtoon(263735)
+    # get_webtoon(263735, merge=True)
```

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/WebtoonOriginalsScraper.py` & `WebtoonScraper-0.1.1/WebtoonScraper/WebtoonOriginalsScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/__init__.py` & `WebtoonScraper-0.1.1/WebtoonScraper/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,10 +2,11 @@
 from WebtoonScraper.foldermanagement import WebtoonFolderManagement
 from WebtoonScraper.WebtoonOriginalsScraper import WebtoonOriginalsScraper
 from WebtoonScraper.BestChallengeScraper import BestChallengeScraper
 from WebtoonScraper.WebtoonCanvasScraper import WebtoonCanvasScraper
 from WebtoonScraper import Webtoon
 from WebtoonScraper.TelescopeScraper import TelescopeScraper
 from WebtoonScraper.BufftoonScraper import BufftoonScraper
+from WebtoonScraper.NaverPostScraper import NaverPostScraper
 
 if __name__ == '__main__':
     print('Testing codes.')
```

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper/foldermanagement.py` & `WebtoonScraper-0.1.1/WebtoonScraper/foldermanagement.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 0.1.0a1
+Version: 0.1.1
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
-Keywords: Webtoon,Webtoon Scraper,Never Webtoon,Webtoon Downloader,Download Webtoon
+Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon,demjson3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다. 그 외에도 웹툰 모아서 보기 등 몇 가지 편의 기능을 지원합니다.
@@ -31,52 +31,103 @@
 
    또는
 
    ```
    pip3 install -U WebtoonScraper
    ```
 
-# 웹툰 다운로드하기
-
+# 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경 다운로드하기
+버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/titleid_from_nw.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_webtoon.png)
    국내의 경우 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/title_no_from_webtoons.com.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/webtoons_original.png)
    해외의 경우는 여기에서,
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/number_from_manhwakyung.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/manhwakyung.png)
    만화경의 경우는 여기에서 확인할 수 있습니다.
-2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스 모두 가능합니다.
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
    wt.get_webtoon(76648, wt.N) # titleid를 여기에다 붙여넣으세요.
    # 베스트 도전만화
    wt.get_webtoon(763952, wt.B) # titleid를 여기에다 붙여넣으세요.
-   # 해외 웹툰 오리지널
+   # 웹툰 오리지널
    wt.get_webtoon(1435, wt.O) # titleid를 여기에다 붙여넣으세요.
-   # 해외 웹툰 캔버스
+   # 웹툰 캔버스
    wt.get_webtoon(304446, wt.C) # titleid를 여기에다 붙여넣으세요.
    # 만화경
    wt.get_webtoon(146, wt.M) # titleid를 여기에다 붙여넣으세요. Webtoon.T 태그도 사용 가능합니다.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
    cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 하지만 이 방식은 서로 다른 사이트에서 id가 겹치는 웹툰이 존재하면 오작동할 수 있으니 꼭 태그를 붙이는 것을 추천합니다.
 
-   또 merge 태그를 이용하면
+   또 merge 태그를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 자동으로 5화씩 묶습니다.
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 중간에 웹툰 다운로드가 멈춘 듯이 보여도 정상입니다. 그대로 가만히 있으면 다운로드가 다시 진행됩니다.
 * 만약 작동하지 않는다면 윈도우에서 Python 3.11.3을 설치하고 앞의 과정을 반복해 보세요.
 
+# 버프툰 다운로드하기
+## 로그인하지 않은 상태에서 웹툰 다운로드하기(추천하지 않음)
+로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 웹툰 수가 매우 적기에 추천하지 않습니다.
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+
+   wt.get_webtoon(1007888, wt.BU) # 복사했던 숫자를 여기에다 붙여넣으세요.
+   ```
+3. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 그냥 enter를 눌러줍니다.
+4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
+## 로그인한 상태에서 웹툰 다운로드하기
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 숫자를 복사합니다.
+2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 아무 웹툰이나 들어갑니다.
+3. 아무 요청이나 클릭하고 나온 창에 '머리글' 탭을 엽니다.
+4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
+5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+
+   wt.get_webtoon(1007888, wt.BU) # 첫 번째로 복사했던 숫자를 여기에다 붙여넣으세요.
+   ```
+6. 'Enter cookie of 1007888(시리즈 id) (Enter nothing to preceed without cookie)'라는 문구와 함께 입력란이 나오면 두 번째로 복사했던 일련의 문자열을 붙여넣기합니다.
+4. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+# 네이버 포스트 다운로드하기
+
+1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png)
+<!-- 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+
+   wt.get_post(597061, 19803452) # seriesNo와 memberNo를 차례대로 입력해주세요.
+   ``` -->
+2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+
+   wt.get_webtoon(597061, wt.M) # 우선 seriesNo만 여기에 입력해주세요.
+   ```
+3. 'Enter memberNo of 597061(해당 웹툰의 seriesNo)'라는 말과 함께 입력란이 나오면 거기에 아까 복사해 놓은 memberNo를 붙여넣습니다.
+   ```
+   Enter memberNo 19803452
+   ...진행됨...
+   ```
+4. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
+## 주의사항
+* get_webtoon이 **아닌** get_post 함수를 사용한다는 점을 주의하세요.
+* 웹툰 태그(Webtoon.P)를 작성할 필요가 없으며 작성하면 오류가 난다는 점을 주의하세요.
+* 가끔씩 이유 없는 오류가 발생할 수 있습니다. 
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import *
 
@@ -113,14 +164,22 @@
 
 ### ID를 회차 번호로 그대로 사용하는 이유
 
 우선 작가가 설정한 회차 번호에 맞추는 것은 힘듭니다. 우선 번호가 어디에 있을지 알기 어렵고, 프롤로그가 있을지 없을지 알 수 없으며, 여러 화에 걸쳐 같은 에피소드를 진행하는 경우도 있고, 외전으로 본편의 회차에서 분리된 화를 운영하는 경우가 있어 화에 맞추어서 번호를 정하는 것을 어렵습니다.
 1부터 시작해서 끝까지 일정한 번호를 유지하는 것도 고려해볼 만하나 만약 그렇게 된다면 무결성 체크를 사용하기 어렵게 됩니다.
 따라서 작가가 설정한 회차를 그대로 사용하는 것도 어렵고, 만약 가능하다 할 지라도 무결성 체크를 포기하기 어렵기 때문에 현재는 ID를 회차 번호로 사용하고 있습니다.
 
-## 전 버전과의 차이
+# Relese Note
+
+0.1.1: 네이버 포스트 추가, readme 작성, pbar 표시 내용 변경, 버그 수정
+
+0.1.0: 버프툰 추가, 빠진 부분 재추가
 
 0.0.19.3: merge 속성 추가, get_webtoon 함수로 변경
+
 0.0.19.1: pbar에 표시되는 내용 변경, 내부적 개선
+
 0.0.18: 만화경 지원, 리팩토링됨(Scraper Abstract Base Class 추가)
+
 0.0.17: 웹툰즈 오리지널, 캔버스 지원
+
 0.0.12: 네이버 웹툰, 베스트 도전 지원
```

### Comparing `WebtoonScraper-0.1.0a1/WebtoonScraper.egg-info/SOURCES.txt` & `WebtoonScraper-0.1.1/WebtoonScraper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
-number_from_manhwakyung.png
 setup.py
-title_no_from_webtoons.com.png
-titleid_from_nw.png
 WebtoonScraper/BestChallengeScraper.py
 WebtoonScraper/BufftoonScraper.py
+WebtoonScraper/NaverPostScraper.py
 WebtoonScraper/NaverWebtoonScraper.py
 WebtoonScraper/Scraper.py
 WebtoonScraper/TelescopeScraper.py
 WebtoonScraper/Webtoon.py
 WebtoonScraper/WebtoonCanvasScraper.py
 WebtoonScraper/WebtoonOriginalsScraper.py
 WebtoonScraper/__init__.py
```

### Comparing `WebtoonScraper-0.1.0a1/setup.py` & `WebtoonScraper-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from setuptools import setup, find_packages
 
-# this_directory = Path(__file__).parent
-# long_description = (this_directory / "README.md").read_text()
-
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = '이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.\n'
     long_description += f.read()
-    long_description = long_description.replace('titleid_from_nw.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/titleid_from_nw.png')
-    long_description = long_description.replace('title_no_from_webtoons.com.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/title_no_from_webtoons.com.png')
-    long_description = long_description.replace('number_from_manhwakyung.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/number_from_manhwakyung.png')
+    long_description = long_description.replace('naver_webtoon.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_webtoon.png')
+    long_description = long_description.replace('webtoons_original.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/webtoons_original.png')
+    long_description = long_description.replace('manhwakyung.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/manhwakyung.png')
+    long_description = long_description.replace('naver_post.png', 'https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/naver_post.png')
 
 setup(
     name='WebtoonScraper',
-    version='0.1.0-alpha1',
+    version='0.1.1',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
-    install_requires=['tqdm', 'bs4', 'requests', 'better_abc'],
+    install_requires=['tqdm', 'bs4', 'requests', 'better_abc', 'async_lru'],
     packages=find_packages(exclude=[]),
-    keywords=['Webtoon', 'Webtoon Scraper', 'Never Webtoon', 'Webtoon Downloader', 'Download Webtoon'],
-    python_requires='>=3.8',
+    keywords=['Webtoon', 'Webtoon Scraper', 'Naver Webtoon', 'Webtoon Downloader', 'Download Webtoon', 'demjson3'],
+    python_requires='>=3.10',
     package_data={},
     zip_safe=False,
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

