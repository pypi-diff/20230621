# Comparing `tmp/karoto-0.1.tar.gz` & `tmp/karoto-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karoto-0.1.tar", max compression
+gzip compressed data, was "karoto-0.2.tar", max compression
```

## Comparing `karoto-0.1.tar` & `karoto-0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1056 2023-04-01 10:24:23.341119 karoto-0.1/LICENSE.MIT
--rw-r--r--   0        0        0      627 2023-04-01 10:24:23.341119 karoto-0.1/LICENSE.anarchist.md
--rw-r--r--   0        0        0     4044 2023-04-02 07:45:52.165317 karoto-0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-01 10:24:23.341119 karoto-0.1/karoto/__init__.py
--rw-r--r--   0        0        0     7948 2023-04-01 10:24:23.341119 karoto-0.1/karoto/backend.py
--rw-r--r--   0        0        0     2751 2023-04-01 10:24:23.341119 karoto-0.1/karoto/base_feed.py
--rw-r--r--   0        0        0      573 2023-04-01 10:24:23.345119 karoto-0.1/karoto/clickable_label.py
--rwxr-xr-x   0        0        0     2533 2023-04-01 10:24:23.345119 karoto-0.1/karoto/error_bar.py
--rwxr-xr-x   0        0        0     4683 2023-04-01 10:24:23.345119 karoto-0.1/karoto/main.py
--rw-r--r--   0        0        0     7862 2023-04-01 10:24:23.345119 karoto-0.1/karoto/shopping_feed.py
--rw-r--r--   0        0        0    10385 2023-04-01 10:24:23.345119 karoto-0.1/karoto/storage_feed.py
--rw-r--r--   0        0        0     1406 2023-04-01 10:24:23.349119 karoto-0.1/karoto/style.py
--rw-r--r--   0        0        0      721 2023-04-01 20:19:41.697602 karoto-0.1/pyproject.toml
--rw-r--r--   0        0        0     4656 1970-01-01 00:00:00.000000 karoto-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-01 10:24:23.341119 karoto-0.2/LICENSE.MIT
+-rw-r--r--   0        0        0      627 2023-04-01 10:24:23.341119 karoto-0.2/LICENSE.anarchist.md
+-rw-r--r--   0        0        0     4588 2023-06-21 18:08:59.142683 karoto-0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-01 10:24:23.341119 karoto-0.2/karoto/__init__.py
+-rw-r--r--   0        0        0    10577 2023-05-24 15:48:00.283652 karoto-0.2/karoto/backend.py
+-rw-r--r--   0        0        0     2751 2023-04-01 10:24:23.341119 karoto-0.2/karoto/base_feed.py
+-rw-r--r--   0        0        0      573 2023-04-01 10:24:23.345119 karoto-0.2/karoto/clickable_label.py
+-rw-r--r--   0        0        0     2533 2023-05-24 15:48:00.287652 karoto-0.2/karoto/error_bar.py
+-rw-r--r--   0        0        0    11302 2023-05-24 15:48:00.287652 karoto-0.2/karoto/flow_layout.py
+-rwxr-xr-x   0        0        0     6381 2023-05-31 18:44:43.957936 karoto-0.2/karoto/main.py
+-rw-r--r--   0        0        0     8353 2023-05-24 15:48:00.287652 karoto-0.2/karoto/shopping_feed.py
+-rw-r--r--   0        0        0    12738 2023-05-25 10:13:11.378138 karoto-0.2/karoto/storage_feed.py
+-rw-r--r--   0        0        0     7369 2023-05-31 18:44:43.957936 karoto-0.2/karoto/style.py
+-rw-r--r--   0        0        0     4491 2023-05-25 09:17:43.797767 karoto-0.2/karoto/tags.py
+-rw-r--r--   0        0        0      721 2023-06-21 18:08:59.142683 karoto-0.2/pyproject.toml
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 karoto-0.2/PKG-INFO
```

### Comparing `karoto-0.1/LICENSE.MIT` & `karoto-0.2/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `karoto-0.1/LICENSE.anarchist.md` & `karoto-0.2/LICENSE.anarchist.md`

 * *Files identical despite different names*

### Comparing `karoto-0.1/README.md` & `karoto-0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,38 +2,53 @@
 
 A Linux mobile app that helps you with your groceries.
 
 It is not just a fancy replacement for your notes app but instead works a bit like a stock management software.
 The heart of the app is a list with things you always want to have at home.
 Before you go to the grocery store or whereever you get your stuff from you can go through this list and check for every item how much you have in your storage.
 The app then generates the shopping list for you which makes it impossible to forget anything.
+
+## Additional features
+- **only once:**
 If you need something like a new knive or some new plates e.g. there is the "only once" option where the item automatically gets deleted as soon as you got it once.
+- **tags:**
+You can add tags to your items and filter for them.
+One example workflow could be to tag everything thats in the fridge with a tag called "Fridge" and when you check whats missing you filter for fridge stuff and only open the fridge once.
+The same can be done while shopping: Tag items for where you can get them and click on the tag when you are there.
+- **hide temporary:**
+Imagine you have a long shopping list but not enough money with you or some items would be to heavy/big to carry so you decide to get it next time.
+Now you can click on the *Hide temporary* button and the item disappears until you restart the app so it does not annoy you.
 
 # Screenshots
-Left/Top: Storage Feed (you go through this list at home), Right/Bottom: Shopping Feed (for in the store e.g.)
-
-![Storage Feed](screenshots/storage_feed.png) ![Shopping Feed](screenshots/shopping_feed.png)
-
-The screenshots were created by gnome-screenshot on a PinePhone with Arch Linux ARM (DanctNIX) installed.
-The software gets also tested on a OnePlus 6 with postmarketOS edge.
-Both devices are running Phosh at the moment.
+#### Storage Feed (you go through this list at home):
+![Storage Feed](screenshots/storage_feed.png)
+#### Shopping Feed (for in the store e.g.):
+![Shopping Feed](screenshots/shopping_feed.png)
+#### Storage Feed filtered for the tag called `Vegetables`:
+![Tags](screenshots/tags.png)
 
 # Installing
 
 Karoto depends on python3 and PyQt6 to run.
 All instructions assume you have cloned the repository and are in its root folder:
 ```
 git clone https://codeberg.org/DrRac27/karoto.git
 cd karoto
 ```
 
 ## No installing
 Without installing you can use `./helper.sh run` to start and test the app.
 
-## Using pip (the easiest if you are not using Arch Linux)
+## Flatpak (the easiest if you are not using Arch Linux)
+Karoto is on Flathub: https://flathub.org/apps/details/page.codeberg.DrRac27.Karoto
+
+## Using pip
+Note: It seems like the dependency PyQt6 is not (yet?) available for ARM via pip.
+You should be able to install it if you add `--no-deps` to the pip command and install the dependencies manually (your package manager probably has PyQt6).
+
 First make sure you have [pip installed](https://packaging.python.org/en/latest/guides/installing-using-linux-tools/#installing-pip-setuptools-wheel-with-linux-package-managers) and then:
 ```
 sudo pip install karoto
 sudo install -Dm 644 packaging/karoto.desktop /usr/share/applications/
 sudo install -Dm 644 packaging/karoto.svg /usr/share/icons/hicolor/scalable/apps/
 ```
 This will install it system-wide.
@@ -50,20 +65,18 @@
 If you e.g. use yay:
 ```
 yay -S karoto
 ```
 If you want to change something before installing there is also a PKGBUILD in `packaging/archlinux` (like for postmarketOS) that you can install using the helper script.
 
 # Roadmap aka some ideas that may get implemented soon™ (by you?)
-- Tags: For example you can tag your items with "Hygiene" or "Fruits/Vegetables" and when you are in the supermarket you can filter your list for the department where you are at that moment. Tags like "Fridge" or "Storage Area" will help while you are putting your list together at home. Or maybe you want to create tags for suppliers?
 - Translation
 - Feedback via feedbackd
 - More styles? Dark style? Custom user styles?
 - Multiple lists to choose from via GUI (already supported via CLI)?
-- Flatpak?
 - support for Android (F-Droid)? PRs welcome! (pyqtdeploy?)
 
 
 # Dev Notes
 - if you want git to stop annoying you with the changed tests/data files you can use
 ```
 git update-index --assume-unchanged <file>
```

### Comparing `karoto-0.1/karoto/backend.py` & `karoto-0.2/karoto/backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,38 +14,43 @@
     _name: str = field(init=False, repr=False, default="")
     wanted: float
     _wanted: float = field(init=False, repr=False, default=1)
     in_stock: float
     _in_stock: float = field(init=False, repr=False, default=0)
     unit: str = ""
     only_once: bool = False
+    tags: list[str]
+    _tags: list[str] = field(init=False, repr=False)
     mtime: float | None = None
+    hidden_temporary: bool = False
 
     def __post_init__(self) -> None:
         if self.mtime is None:
             self._on_change()
 
     def __dict__(self) -> dict:
         return {
             "name": self.name,
             "wanted": self.wanted,
             "in_stock": self.in_stock,
             "unit": self.unit,
             "only_once": self.only_once,
+            "tags": self.tags,
             "mtime": self.mtime,
         }
 
     @classmethod
     def from_dict(cls, d) -> "CartItem":
         return cls(
             name=d["name"],
             wanted=d["wanted"],
             in_stock=d["in_stock"],
             unit=d["unit"],
             only_once=d.get("only_once", False),
+            tags=d.get("tags", list()),
             mtime=d.get("mtime", 0),
         )
 
     def __eq__(self, other) -> bool:
         """Attention: Ignores mtime!"""
         if self.name != other.name:
             return False
@@ -53,25 +58,30 @@
             return False
         if self.in_stock != other.in_stock:
             return False
         if self.unit != other.unit:
             return False
         if self.only_once != other.only_once:
             return False
+        if self.tags != other.tags:
+            return False
+        if self.hidden_temporary != other.hidden_temporary:
+            return False
         return True
 
     @property
     def name(self) -> str:
         return self._name
 
     @name.setter
     def name(self, new: str) -> None:
         if type(new) is property:
             # initial value not specified, use default
-            new = CartItem._name
+            self._name = CartItem._name
+            return
 
         if type(new) != str:
             raise ValueError()
 
         if self._name == new:
             return
 
@@ -82,15 +92,16 @@
     def in_stock(self) -> float | int:
         return self._int_if_possible(self._in_stock)
 
     @in_stock.setter
     def in_stock(self, new: any) -> None:
         if type(new) is property:
             # initial value not specified, use default
-            new = CartItem._in_stock
+            self._in_stock = CartItem._in_stock
+            return
 
         new = self._to_float(new)
 
         if new < 0:
             raise ValueError("Negative numbers are not supported!")
 
         if new == self.in_stock:
@@ -103,15 +114,16 @@
     def wanted(self) -> float | int:
         return self._int_if_possible(self._wanted)
 
     @wanted.setter
     def wanted(self, new):
         if type(new) is property:
             # initial value not specified, use default
-            new = CartItem._wanted
+            self._wanted = CartItem._wanted
+            return
 
         new = self._to_float(new)
 
         if self._wanted == new:
             return
 
         if new <= 0:
@@ -140,14 +152,43 @@
     def needs_restock(self) -> bool:
         return self.wanted > self.in_stock
 
     @property
     def is_dead(self) -> bool:
         return self.only_once and not self.needs_restock
 
+    @property
+    def tags(self) -> list[str]:
+        """There is a problem with mutable properties like lists:
+        If you use e.g. item.tags.append() the setter does not get called.
+        To at least make this a more obvious bug we return a copy of the list
+        using [:] so .append() will not work. """
+        return self._tags[:]
+
+    @tags.setter
+    def tags(self, new) -> None:
+        if type(new) is property:
+            # initial value not specified, use default
+            self._tags = []
+            return
+
+        if getattr(self, "_tags", None) == new:
+            return
+
+        self._tags = new
+        self._on_change()
+
+    def add_tag(self, name) -> None:
+        self._tags.append(name)
+        self._on_change()
+
+    def remove_tag(self, name) -> None:
+        self._tags.remove(name)
+        self._on_change()
+
     def _on_change(self) -> None:
         self.mtime = time()
 
     def bought_all(self) -> None:
         self.in_stock = self.wanted
 
     def _int_if_possible(self, value: float) -> float | int:
@@ -240,37 +281,91 @@
     def save_list(self, list_name: str = None, full_path: str = None) -> None:
         self.fm.save_list(
             self.storage,
             name=list_name,
             full_path=full_path,
         )
 
-    def _get_filtered_items(self, search: str = None) -> list:
-        if not search:
+    def _get_filtered_items(
+            self,
+            search: str = "",
+            filter_tags: list[str] = [],
+            ) -> list:
+
+        if search == "" and filter_tags == []:
             ret = self.storage
             ret.sort(key=lambda k: k.mtime, reverse=True)
             return ret
 
         new_list = list()
         for item in self.storage:
-            if item.name.lower().find(search.lower()) != -1:
+            if search != "" and item.name.lower().find(search.lower()) == -1:
+                continue
+
+            found_missing = False
+            for tag in filter_tags:
+                if tag not in item.tags:
+                    found_missing = True
+                    break
+            if not found_missing:
                 new_list.append(item)
+
         new_list.sort(key=lambda k: k.mtime, reverse=True)
         return new_list
 
-    def get_items_in_stock(self, search: str = None) -> list:
-        return self._get_filtered_items(search=search)
+    def get_items_in_stock(
+            self,
+            search: str = "",
+            filter_tags: list[str] = [],
+            ) -> list:
+
+        return self._get_filtered_items(search=search, filter_tags=filter_tags)
+
+    def get_items_to_buy(
+            self,
+            search: str = "",
+            filter_tags: list[str] = [],
+            ) -> list:
 
-    def get_items_to_buy(self, search: str = None) -> list:
         items = list()
-        for item in self._get_filtered_items(search=search):
-            if item.needs_restock:
+        for item in self._get_filtered_items(
+                search=search,
+                filter_tags=filter_tags,
+                ):
+            if item.needs_restock and not item.hidden_temporary:
                 items.append(item)
         return items
 
+    def get_tags(
+            self,
+            search: str = "",
+            filter_tags: list[str] = [],
+            storage_mode=True,
+            ) -> list[tuple[str, int]]:
+        if storage_mode:
+            all_items = self.get_items_in_stock(
+                search=search,
+                filter_tags=filter_tags,
+            )
+        else:
+            all_items = self.get_items_to_buy(
+                search=search,
+                filter_tags=filter_tags,
+            )
+
+        all_tags = []
+        for item in all_items:
+            all_tags += item.tags
+
+        counted_tags = []
+        for tag in set(all_tags):
+            counted_tags.append((tag, all_tags.count(tag)))
+
+        return counted_tags
+
     def add_item(self, item: CartItem):
         if self.get_item_by_name(item.name) is not None:
             raise DuplicateError("A item with this name already exists")
         self.storage.append(item)
 
     def delete(self, item: CartItem) -> None:
         self.storage.remove(item)
```

### Comparing `karoto-0.1/karoto/base_feed.py` & `karoto-0.2/karoto/base_feed.py`

 * *Files identical despite different names*

### Comparing `karoto-0.1/karoto/clickable_label.py` & `karoto-0.2/karoto/clickable_label.py`

 * *Files identical despite different names*

### Comparing `karoto-0.1/karoto/error_bar.py` & `karoto-0.2/karoto/error_bar.py`

 * *Files identical despite different names*

### Comparing `karoto-0.1/karoto/shopping_feed.py` & `karoto-0.2/karoto/shopping_feed.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,22 +16,26 @@
 from karoto.clickable_label import ClickableLabel
 from karoto.base_feed import BaseFeed
 
 
 class ShoppingFeedItemDetails(QWidget):
     item_changed = pyqtSignal()
     warn_message = pyqtSignal(str)
+    needs_reload = pyqtSignal()
 
     def __init__(self, item: CartItem) -> None:
         super().__init__()
         self.item = item
 
         self.init_ui()
 
     def init_ui(self) -> None:
+        self.hide_button = QPushButton("Hide temporary")
+        self.hide_button.clicked.connect(self.hide_temporary)
+
         self.minus_button = QPushButton("-")
         self.minus_button.clicked.connect(self.decrease)
         self.minus_button.setProperty("class", "single_char_button")
 
         self.missing_edit = QLineEdit("ERROR")
         self.missing_edit.editingFinished.connect(self.update_missing)
         self.missing_edit.setSizePolicy(
@@ -44,14 +48,15 @@
 
         self.plus_button = QPushButton("+")
         self.plus_button.clicked.connect(self.increase)
         self.plus_button.setProperty("class", "single_char_button")
 
         self.layout_ = QHBoxLayout()
         self.layout_.addStretch()
+        self.layout_.addWidget(self.hide_button)
         self.layout_.addWidget(self.minus_button)
         self.layout_.addWidget(self.missing_edit)
         self.layout_.addWidget(self.wanted_label)
         self.layout_.addWidget(self.plus_button)
         self.setLayout(self.layout_)
 
     def reload(self) -> None:
@@ -91,19 +96,24 @@
         self.item.missing += 1
         self.item_changed.emit()
 
     def decrease(self) -> None:
         self.item.missing -= 1
         self.item_changed.emit()
 
+    def hide_temporary(self) -> None:
+        self.item.hidden_temporary = True
+        self.needs_reload.emit()
+
 
 class ShoppingFeedItem(QGroupBox):
     item_changed = pyqtSignal()
     bought_all = pyqtSignal()
     warn_message = pyqtSignal(str)
+    needs_reload = pyqtSignal()
 
     def __init__(self, item: CartItem) -> None:
         super().__init__()
         self.item = item
 
         self.init_ui()
 
@@ -146,14 +156,15 @@
 
     def _init_details(self) -> None:
         """details get initialized when needed only to speed up the app"""
         self.details = ShoppingFeedItemDetails(self.item)
         self.details.item_changed.connect(self.item_changed)
         self.details.item_changed.connect(self.check_bought_all)
         self.details.item_changed.connect(self.reload)
+        self.details.needs_reload.connect(self.needs_reload)
         self.details.warn_message.connect(self.warn_message)
         self.details.setHidden(True)
         self.layout_.addWidget(self.details)
 
     def check_bought_all(self) -> None:
         if not self.item.needs_restock:
             self.bought_all.emit()
@@ -185,14 +196,15 @@
         self.details.setHidden(not self.details.isHidden())
         self.reload()
 
 
 class ShoppingFeed(BaseFeed):
     item_changed = pyqtSignal(CartItem)
     warn_message = pyqtSignal(str)
+    needs_reload = pyqtSignal()
 
     def init_ui(self) -> None:
         self.scroll_widget = QWidget()
         self.scroll_layout = QVBoxLayout()
         self.item_layout = QVBoxLayout()
         self.scroll_layout.addLayout(self.item_layout)
         self.scroll_layout.addStretch(1)
@@ -209,14 +221,15 @@
             self.viewport(), QScroller.ScrollerGestureType.TouchGesture
         )
 
     def _create_ui_item(self, item: CartItem) -> ShoppingFeedItem:
         si = ShoppingFeedItem(item)
         si.item_changed.connect(lambda x=item: self.item_changed.emit(x))
         si.bought_all.connect(lambda x=item: self.remove_item(x))
+        si.needs_reload.connect(self.needs_reload)
         si.warn_message.connect(self.warn_message)
         return si
 
 
 def main() -> None:
     app = QApplication(sys.argv)
     cart_items = [
```

### Comparing `karoto-0.1/karoto/storage_feed.py` & `karoto-0.2/karoto/storage_feed.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,50 +13,61 @@
     QVBoxLayout,
     QWidget,
 )
 from PyQt6.QtCore import pyqtSignal, Qt
 from karoto.backend import CartItem
 from karoto.clickable_label import ClickableLabel
 from karoto.base_feed import BaseFeed
+from karoto.tags import Tags
 
 
 class StorageFeedItemDetails(QWidget):
     item_saved = pyqtSignal()
     item_deleted = pyqtSignal()
     name_changed = pyqtSignal(str)
 
     def __init__(self, item: CartItem, is_for_wizzard=False) -> None:
         super().__init__()
         self.item = item
+        self.last_saved_tags = item.tags  # TODO: Hacky...
         self.is_for_wizzard = is_for_wizzard
 
         self.init_ui()
 
     def init_ui(self) -> None:
         self.layout_ = QGridLayout()
         self.setLayout(self.layout_)
 
         self.name_label = QLabel("Name:")
         self.name_edit = QLineEdit("ERROR")
+        self.name_edit.textChanged.connect(self.check_changes)
 
         self.in_stock_label = QLabel("In stock:")
         self.in_stock_edit = QLineEdit("ERROR")
+        self.in_stock_edit.textChanged.connect(self.check_changes)
 
         self.wanted_label = QLabel("Wanted:")
         self.wanted_edit = QLineEdit("ERROR")
+        self.wanted_edit.textChanged.connect(self.check_changes)
 
         self.unit_label = QLabel("Unit:")
         self.unit_edit = QLineEdit("ERROR")
+        self.unit_edit.textChanged.connect(self.check_changes)
 
         self.only_once_label = QLabel("Only Once:")
         self.only_once_check = QCheckBox()
+        self.only_once_check.toggled.connect(self.check_changes)
+
+        self.tags_label = QLabel("Tags:")
+        self.init_tags()
 
         self.save_button = QPushButton(
             "Create Item" if self.is_for_wizzard else "Save"
         )
+        self.save_button.setEnabled(False)
         self.save_button.clicked.connect(self.save_changes)
 
         if not self.is_for_wizzard:
             self.delete_button = QPushButton("Delete")
             self.delete_button.clicked.connect(self.item_deleted)
 
         self.layout_.addWidget(self.name_label, 0, 0)
@@ -65,41 +76,96 @@
         self.layout_.addWidget(self.in_stock_edit, 1, 1)
         self.layout_.addWidget(self.wanted_label, 2, 0)
         self.layout_.addWidget(self.wanted_edit, 2, 1)
         self.layout_.addWidget(self.unit_label, 3, 0)
         self.layout_.addWidget(self.unit_edit, 3, 1)
         self.layout_.addWidget(self.only_once_label, 4, 0)
         self.layout_.addWidget(self.only_once_check, 4, 1)
-        self.layout_.addWidget(self.save_button, 5, 1)
+        self.layout_.addWidget(self.tags_label, 5, 0)
+        self.layout_.addWidget(self.save_button, 6, 1)
         if not self.is_for_wizzard:
-            self.layout_.addWidget(self.delete_button, 6, 1)
+            self.layout_.addWidget(self.delete_button, 7, 1)
 
         self.reload()
 
+    def init_tags(self) -> None:
+        self.tags_widget = Tags(self.item.tags)
+        self.layout_.addWidget(self.tags_widget, 5, 1)
+        self.tags_widget.created_tag.connect(self.create_tag)
+        self.tags_widget.created_tag.connect(self.check_changes)
+        self.tags_widget.deleted_tag.connect(self.delete_tag)
+        self.tags_widget.deleted_tag.connect(self.check_changes)
+
     def reload(self) -> None:
         self.name_edit.setText(self.item.name)
         self.in_stock_edit.setText(str(self.item.in_stock))
         self.wanted_edit.setText(str(self.item.wanted))
         self.unit_edit.setText(self.item.unit)
         self.only_once_check.setChecked(self.item.only_once)
+        self.reload_tags()
+
+    def reload_tags(self):
+        self.layout_.removeWidget(self.tags_widget)
+        self.tags_widget.deleteLater()
+        self.init_tags()
+
+    def create_tag(self, name) -> None:
+        self.item.add_tag(name)
+        self.reload_tags()
+
+    def delete_tag(self, name) -> None:
+        self.item.remove_tag(name)
+        self.reload_tags()
+
+    def check_changes(self) -> None:
+        found_changes = False
+
+        if self.item.name != self.name_edit.text():
+            found_changes = True
+
+        try:
+            if self.item.in_stock != float(self.in_stock_edit.text()):
+                found_changes = True
+        except ValueError:
+            pass
+
+        try:
+            if self.item.wanted != float(self.wanted_edit.text()):
+                found_changes = True
+        except ValueError:
+            pass
+
+        if self.item.unit != self.unit_edit.text():
+            found_changes = True
+
+        if self.item.only_once != self.only_once_check.isChecked():
+            found_changes = True
+
+        if self.last_saved_tags != self.tags_widget.tags:
+            found_changes = True
+
+        self.save_button.setEnabled(found_changes)
 
     def save_changes(self) -> None:
         new_name = self.name_edit.text()
         if self.is_for_wizzard:
             self.item.name = new_name
         elif self.item.name != new_name:
             self.name_changed.emit(new_name)
 
         self.item.in_stock = self.in_stock_edit.text()
         self.item.wanted = self.wanted_edit.text()
         self.item.unit = self.unit_edit.text()
         self.item.only_once = self.only_once_check.isChecked()
+        self.last_saved_tags = self.item.tags
 
         self.item_saved.emit()
 
+        self.save_button.setEnabled(False)
+
 
 class StorageFeedItem(QGroupBox):
     item_changed = pyqtSignal()
     item_deleted = pyqtSignal()
     name_changed = pyqtSignal(str)
     warn_message = pyqtSignal(str)
 
@@ -146,21 +212,23 @@
 
         self.top_layout.addWidget(self.name_label)
         self.top_layout.addWidget(self.minus_button)
         self.top_layout.addWidget(self.in_stock_edit)
         self.top_layout.addWidget(self.wanted_label)
         self.top_layout.addWidget(self.plus_button)
 
+        self.item_changed.connect(self.reload)
         self.reload()
 
     def _init_details(self) -> None:
         """details get initialized only when needed to speed up the app"""
 
         self.details = StorageFeedItemDetails(item=self.item)
         self.details.item_saved.connect(self.item_changed)
+        self.details.item_saved.connect(self.toggle_details)
         self.details.item_deleted.connect(self.item_deleted)
         self.details.name_changed.connect(self.name_changed)
         self.details.setHidden(True)
         self.layout_.addWidget(self.details)
 
     def reload(self) -> None:
         self.name_label.setText(self.item.name)
```

### Comparing `karoto-0.1/pyproject.toml` & `karoto-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "karoto"
-version = "0.1"
+version = "0.2"
 description = "A shopping list app for Linux Mobile"
 authors = ["DrRac27 <drrac27@riseup.net>"]
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `karoto-0.1/PKG-INFO` & `karoto-0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 Metadata-Version: 2.1
 Name: karoto
-Version: 0.1
+Version: 0.2
 Summary: A shopping list app for Linux Mobile
 Keywords: shopping,list,carrot,storage,stock,management,cart,basket
 Author: DrRac27
 Author-email: drrac27@riseup.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: pyqt6 (>=6.4.2,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Karoto Shopping List
 
 A Linux mobile app that helps you with your groceries.
 
 It is not just a fancy replacement for your notes app but instead works a bit like a stock management software.
 The heart of the app is a list with things you always want to have at home.
 Before you go to the grocery store or whereever you get your stuff from you can go through this list and check for every item how much you have in your storage.
 The app then generates the shopping list for you which makes it impossible to forget anything.
+
+## Additional features
+- **only once:**
 If you need something like a new knive or some new plates e.g. there is the "only once" option where the item automatically gets deleted as soon as you got it once.
+- **tags:**
+You can add tags to your items and filter for them.
+One example workflow could be to tag everything thats in the fridge with a tag called "Fridge" and when you check whats missing you filter for fridge stuff and only open the fridge once.
+The same can be done while shopping: Tag items for where you can get them and click on the tag when you are there.
+- **hide temporary:**
+Imagine you have a long shopping list but not enough money with you or some items would be to heavy/big to carry so you decide to get it next time.
+Now you can click on the *Hide temporary* button and the item disappears until you restart the app so it does not annoy you.
 
 # Screenshots
-Left/Top: Storage Feed (you go through this list at home), Right/Bottom: Shopping Feed (for in the store e.g.)
-
-![Storage Feed](screenshots/storage_feed.png) ![Shopping Feed](screenshots/shopping_feed.png)
-
-The screenshots were created by gnome-screenshot on a PinePhone with Arch Linux ARM (DanctNIX) installed.
-The software gets also tested on a OnePlus 6 with postmarketOS edge.
-Both devices are running Phosh at the moment.
+#### Storage Feed (you go through this list at home):
+![Storage Feed](screenshots/storage_feed.png)
+#### Shopping Feed (for in the store e.g.):
+![Shopping Feed](screenshots/shopping_feed.png)
+#### Storage Feed filtered for the tag called `Vegetables`:
+![Tags](screenshots/tags.png)
 
 # Installing
 
 Karoto depends on python3 and PyQt6 to run.
 All instructions assume you have cloned the repository and are in its root folder:
 ```
 git clone https://codeberg.org/DrRac27/karoto.git
 cd karoto
 ```
 
 ## No installing
 Without installing you can use `./helper.sh run` to start and test the app.
 
-## Using pip (the easiest if you are not using Arch Linux)
+## Flatpak (the easiest if you are not using Arch Linux)
+Karoto is on Flathub: https://flathub.org/apps/details/page.codeberg.DrRac27.Karoto
+
+## Using pip
+Note: It seems like the dependency PyQt6 is not (yet?) available for ARM via pip.
+You should be able to install it if you add `--no-deps` to the pip command and install the dependencies manually (your package manager probably has PyQt6).
+
 First make sure you have [pip installed](https://packaging.python.org/en/latest/guides/installing-using-linux-tools/#installing-pip-setuptools-wheel-with-linux-package-managers) and then:
 ```
 sudo pip install karoto
 sudo install -Dm 644 packaging/karoto.desktop /usr/share/applications/
 sudo install -Dm 644 packaging/karoto.svg /usr/share/icons/hicolor/scalable/apps/
 ```
 This will install it system-wide.
@@ -67,20 +81,18 @@
 If you e.g. use yay:
 ```
 yay -S karoto
 ```
 If you want to change something before installing there is also a PKGBUILD in `packaging/archlinux` (like for postmarketOS) that you can install using the helper script.
 
 # Roadmap aka some ideas that may get implemented soon™ (by you?)
-- Tags: For example you can tag your items with "Hygiene" or "Fruits/Vegetables" and when you are in the supermarket you can filter your list for the department where you are at that moment. Tags like "Fridge" or "Storage Area" will help while you are putting your list together at home. Or maybe you want to create tags for suppliers?
 - Translation
 - Feedback via feedbackd
 - More styles? Dark style? Custom user styles?
 - Multiple lists to choose from via GUI (already supported via CLI)?
-- Flatpak?
 - support for Android (F-Droid)? PRs welcome! (pyqtdeploy?)
 
 
 # Dev Notes
 - if you want git to stop annoying you with the changed tests/data files you can use
 ```
 git update-index --assume-unchanged <file>
```

