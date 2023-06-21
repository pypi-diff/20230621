# Comparing `tmp/social-blade-scraper-0.0.5.tar.gz` & `tmp/social-blade-scraper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-blade-scraper-0.0.5.tar", last modified: Wed Jun 21 07:09:28 2023, max compression
+gzip compressed data, was "social-blade-scraper-0.0.6.tar", last modified: Wed Jun 21 09:17:47 2023, max compression
```

## Comparing `social-blade-scraper-0.0.5.tar` & `social-blade-scraper-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 07:09:28.829757 social-blade-scraper-0.0.5/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 07:09:28.829757 social-blade-scraper-0.0.5/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.0.5/README.md
--rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-21 07:09:28.829757 social-blade-scraper-0.0.5/setup.cfg
--rw-rw-r--   0 tej       (1000) tej       (1000)      720 2023-06-21 07:09:18.000000 social-blade-scraper-0.0.5/setup.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 07:09:28.829757 social-blade-scraper-0.0.5/src/
--rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.0.5/src/__init__.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 07:09:28.829757 social-blade-scraper-0.0.5/src/social_blade_scraper/
--rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.0.5/src/social_blade_scraper/__init__.py
--rw-rw-r--   0 tej       (1000) tej       (1000)      809 2023-06-21 03:28:03.000000 social-blade-scraper-0.0.5/src/social_blade_scraper/fetch.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 07:09:28.829757 social-blade-scraper-0.0.5/src/social_blade_scraper/stats/
--rw-rw-r--   0 tej       (1000) tej       (1000)    12410 2023-06-21 03:07:47.000000 social-blade-scraper-0.0.5/src/social_blade_scraper/stats/youtube.py
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 07:09:28.829757 social-blade-scraper-0.0.5/src/social_blade_scraper.egg-info/
--rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 07:09:28.000000 social-blade-scraper-0.0.5/src/social_blade_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 tej       (1000) tej       (1000)      408 2023-06-21 07:09:28.000000 social-blade-scraper-0.0.5/src/social_blade_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-21 07:09:28.000000 social-blade-scraper-0.0.5/src/social_blade_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       39 2023-06-21 07:09:28.000000 social-blade-scraper-0.0.5/src/social_blade_scraper.egg-info/requires.txt
--rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-21 07:09:28.000000 social-blade-scraper-0.0.5/src/social_blade_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 07:09:28.829757 social-blade-scraper-0.0.5/tests/
--rw-rw-r--   0 tej       (1000) tej       (1000)     1752 2023-06-21 03:46:47.000000 social-blade-scraper-0.0.5/tests/test_youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 09:17:47.879702 social-blade-scraper-0.0.6/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 09:17:47.879702 social-blade-scraper-0.0.6/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)       23 2023-06-20 07:41:43.000000 social-blade-scraper-0.0.6/README.md
+-rw-rw-r--   0 tej       (1000) tej       (1000)       38 2023-06-21 09:17:47.879702 social-blade-scraper-0.0.6/setup.cfg
+-rw-rw-r--   0 tej       (1000) tej       (1000)      717 2023-06-21 09:17:41.000000 social-blade-scraper-0.0.6/setup.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 09:17:47.875702 social-blade-scraper-0.0.6/src/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 05:17:33.000000 social-blade-scraper-0.0.6/src/__init__.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 09:17:47.875702 social-blade-scraper-0.0.6/src/social_blade_scraper/
+-rw-rw-r--   0 tej       (1000) tej       (1000)        0 2023-06-20 08:55:41.000000 social-blade-scraper-0.0.6/src/social_blade_scraper/__init__.py
+-rw-rw-r--   0 tej       (1000) tej       (1000)      901 2023-06-21 09:01:45.000000 social-blade-scraper-0.0.6/src/social_blade_scraper/fetch.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 09:17:47.879702 social-blade-scraper-0.0.6/src/social_blade_scraper/stats/
+-rw-rw-r--   0 tej       (1000) tej       (1000)    12339 2023-06-21 09:03:24.000000 social-blade-scraper-0.0.6/src/social_blade_scraper/stats/youtube.py
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 09:17:47.879702 social-blade-scraper-0.0.6/src/social_blade_scraper.egg-info/
+-rw-rw-r--   0 tej       (1000) tej       (1000)      400 2023-06-21 09:17:47.000000 social-blade-scraper-0.0.6/src/social_blade_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 tej       (1000) tej       (1000)      408 2023-06-21 09:17:47.000000 social-blade-scraper-0.0.6/src/social_blade_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)        1 2023-06-21 09:17:47.000000 social-blade-scraper-0.0.6/src/social_blade_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       36 2023-06-21 09:17:47.000000 social-blade-scraper-0.0.6/src/social_blade_scraper.egg-info/requires.txt
+-rw-rw-r--   0 tej       (1000) tej       (1000)       30 2023-06-21 09:17:47.000000 social-blade-scraper-0.0.6/src/social_blade_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 tej       (1000) tej       (1000)        0 2023-06-21 09:17:47.879702 social-blade-scraper-0.0.6/tests/
+-rw-rw-r--   0 tej       (1000) tej       (1000)     1923 2023-06-21 09:08:45.000000 social-blade-scraper-0.0.6/tests/test_youtube.py
```

### Comparing `social-blade-scraper-0.0.5/setup.py` & `social-blade-scraper-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from setuptools import setup
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name="social-blade-scraper",
-    version="0.0.5",
+    version="0.0.6",
     description="Social blade scraper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/tejmagar/social-blade-scraper",
     install_requires=[
         "beautifulsoup4",
-        "requests",
+        "httpx",
         "fake-useragent"
     ],
     package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `social-blade-scraper-0.0.5/src/social_blade_scraper/stats/youtube.py` & `social-blade-scraper-0.0.6/src/social_blade_scraper/stats/youtube.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from concurrent.futures import ThreadPoolExecutor, wait
+import asyncio
 from typing import Union, List, Tuple
 
 from bs4 import BeautifulSoup
 import re
 
 from dataclasses import dataclass, asdict
 
@@ -168,39 +168,39 @@
         )
 
         data.append(record)
 
     return data
 
 
-def fetch_homepage(channel_name: str) -> Union[str, None]:
+async def fetch_homepage(channel_name: str) -> Union[str, None]:
     """
     Returns home page source code
 
     :param channel_name: YouTube channel name
     :return: Union[str, None]
     """
     target_url = f'https://socialblade.com/youtube/c/{channel_name}'
-    response = fetch(target_url)
+    response = await fetch(target_url)
 
-    if response.ok:
+    if response.status_code == 200:
         return response.text
 
 
-def fetch_monthly_page(channel_name: str) -> Union[str, None]:
+async def fetch_monthly_page(channel_name: str) -> Union[str, None]:
     """ Returns source code of monthly stats page
 
     :param channel_name: YouTube channel name
     :return: Union[str, None]
     """
 
     target_url = f'https://socialblade.com/youtube/c/{channel_name}/monthly'
-    response = fetch(target_url)
+    response = await fetch(target_url)
 
-    if response.ok:
+    if response.status_code == 200:
         return response.text
 
 
 def total_uploads_search(soup: BeautifulSoup) -> Union[int, None]:
     """
     Logic to search total uploads
 
@@ -277,23 +277,23 @@
        """
 
     tag = soup.select_one('#youtube-stats-header-channeltype')
     if tag:
         return tag.text.strip()
 
 
-def home_page_scrape(channel_name: str, channel: YouTubeChannel) -> bool:
+async def home_page_scrape(channel_name: str, channel: YouTubeChannel) -> bool:
     """
     Returns True if home page is scraped successfully else false
     :param channel_name: YouTube channel name
     :param channel: temporary channel instance to store information
     :return: bool
     """
 
-    code = fetch_homepage(channel_name)
+    code = await fetch_homepage(channel_name)
     if not code:
         return False
 
     soup = BeautifulSoup(code, 'html.parser')
 
     channel.date_created = date_created_search(soup)
 
@@ -312,59 +312,55 @@
     channel.total_uploads = total_uploads_search(soup)
     channel.total_subscribers = total_subscribers_search(soup)
     channel.total_views = total_views_search(soup)
     channel.country = country_search(soup)
     return True
 
 
-def daily_stats_scrape(channel_name: str) -> List[DailyStat]:
+async def daily_stats_scrape(channel_name: str) -> List[DailyStat]:
     """
     Returns  30 days daily stats
 
     :param channel_name: YouTube channel name
     :return:
     """
 
-    code = fetch_monthly_page(channel_name)
+    code = await fetch_monthly_page(channel_name)
     if not code:
         return []
 
     soup = BeautifulSoup(code, 'html.parser')
     return daily_stats_search(soup)
 
 
-def social_blade_scrape(channel_name: str) -> Union[YouTubeChannel, None]:
+async def social_blade_scrape(channel_name: str) -> Union[YouTubeChannel, None]:
     # Create a BeautifulSoup object with the HTML content
 
-    with ThreadPoolExecutor() as executor:
-        channel = YouTubeChannel()
-        future_homepage_scrape = executor.submit(home_page_scrape, channel_name, channel)
-        future_daily_stats_scrape = executor.submit(daily_stats_scrape, channel_name)
-
-        # Wait for futures to complete
-        wait([future_homepage_scrape, future_daily_stats_scrape])
-
-        # Check if the home page is scraped successfully
-        if not future_homepage_scrape.result():
-            # Maybe got 404 status because channel don't exist or something went wrong
-            return None
+    channel = YouTubeChannel()
+    scrape_tasks = await asyncio.gather(home_page_scrape(channel_name, channel), daily_stats_scrape(channel_name))
+    home_page_scrape_future, daily_stats_scrape_future, = scrape_tasks
+
+    # Check if the home page is scraped successfully
+    if not home_page_scrape_future:
+        # Maybe got 404 status because channel don't exist or something went wrong
+        return None
 
-        channel.daily_stats = future_daily_stats_scrape.result()
-        return channel
+    channel.daily_stats = daily_stats_scrape_future
+    return channel
 
 
 def get_username_from_url(url: str) -> Union[str, None]:
     # Example YouTube channel link: https://www.youtube.com/@MrFeast
     url_split = url.split('@')
 
     if len(url_split) > 0:
         return url_split[-1]
 
 
-def youtube(url: str = None, channel_name: str = None) -> Union[YouTubeChannel, None]:
+async def youtube(url: str = None, channel_name: str = None) -> Union[YouTubeChannel, None]:
     """
     Priority order: channel_name, url
     Start scraping social blade easily.
 
     # Using URL
     >> channel = youtube(url='https://www.youtube.com/@MrFeast')
 
@@ -389,15 +385,15 @@
     if url:
         # Extract username from URL
         channel_name = get_username_from_url(url)
 
     if not channel_name:
         return None
 
-    return social_blade_scrape(channel_name)
+    return await social_blade_scrape(channel_name)
 
 
 def subscribers_count_access_tokens_search(soup: BeautifulSoup) -> Union[Tuple[str, str], None]:
     """
     Finds tokens to access subscribers count page
 
     :param soup: BeautifulSoup object
@@ -407,41 +403,41 @@
     encoded_query = soup.select_one('#rawUser')
     token = soup.select_one('#rawToken')
 
     if encoded_query and token:
         return encoded_query.text.strip(), token.text.strip()
 
 
-def subscribers_count_access_tokens(channel_name: str) -> Union[Tuple[str, str], None]:
+async def subscribers_count_access_tokens(channel_name: str) -> Union[Tuple[str, str], None]:
     target_url = f'https://socialblade.com/youtube/user/{channel_name}/realtime'
-    response = fetch(target_url)
+    response = await fetch(target_url)
 
-    if not response.ok:
+    if not response.status_code == 200:
         return None
 
     code = response.text
     soup = BeautifulSoup(code, 'html.parser')
     return subscribers_count_access_tokens_search(soup)
 
 
-def live_subscriber_count(encoded_query: str, token: str) -> Union[int, None]:
+async def live_subscriber_count(encoded_query: str, token: str) -> Union[int, None]:
     """
     Returns live subscriber number
 
     :param encoded_query User Query
     :param token: View token
     :return: str
     """
 
     url = 'https://bastet.socialblade.com/youtube/lookup'
     params = {
         'query': encoded_query,
         'token': token
     }
 
-    response = fetch(url, params=params, extra_headers={
+    response = await fetch(url, params=params, extra_headers={
         'Origin': 'https://socialblade.com',
         'Referer': 'https://socialblade.com/',
     })
 
-    if response.ok:
+    if response.status_code == 200:
         return int(response.text)
```

