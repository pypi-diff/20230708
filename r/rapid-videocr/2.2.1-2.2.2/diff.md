# Comparing `tmp/rapid_videocr-2.2.1-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14922 bytes, number of entries: 11
--rw-r--r--  2.0 unx      174 b- defN 23-Jun-22 11:18 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx     4798 b- defN 23-Jun-22 11:18 rapid_videocr/main.py
--rw-r--r--  2.0 unx    12743 b- defN 23-Jun-22 11:18 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     2756 b- defN 23-Jun-22 11:18 rapid_videocr/utils.py
--rw-r--r--  2.0 unx     1264 b- defN 23-Jun-22 11:18 rapid_videocr/video_sub_finder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4648 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      934 b- defN 23-Jun-22 11:18 rapid_videocr-2.2.1.dist-info/RECORD
-11 files, 38839 bytes uncompressed, 13332 bytes compressed:  65.7%
+Zip file size: 15659 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      174 b- defN 23-Jul-08 11:12 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx     4798 b- defN 23-Jul-08 11:12 rapid_videocr/main.py
+-rw-r--r--  2.0 unx    13456 b- defN 23-Jul-08 11:12 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     4479 b- defN 23-Jul-08 11:12 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx     1264 b- defN 23-Jul-08 11:12 rapid_videocr/video_sub_finder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-08 11:12 rapid_videocr-2.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4650 b- defN 23-Jul-08 11:12 rapid_videocr-2.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 11:12 rapid_videocr-2.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-08 11:12 rapid_videocr-2.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-08 11:12 rapid_videocr-2.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      934 b- defN 23-Jul-08 11:12 rapid_videocr-2.2.2.dist-info/RECORD
+11 files, 41277 bytes uncompressed, 14069 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
 Filename: rapid_videocr/video_sub_finder.py
 Comment: 
 
-Filename: rapid_videocr-2.2.1.dist-info/LICENSE
+Filename: rapid_videocr-2.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.2.1.dist-info/METADATA
+Filename: rapid_videocr-2.2.2.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.2.1.dist-info/WHEEL
+Filename: rapid_videocr-2.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.2.1.dist-info/entry_points.txt
+Filename: rapid_videocr-2.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.1.dist-info/top_level.txt
+Filename: rapid_videocr-2.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.1.dist-info/RECORD
+Filename: rapid_videocr-2.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/main.py

```diff
@@ -9,127 +9,127 @@
 from .utils import get_logger
 from .video_sub_finder import VideoSubFinder
 
 
 class RapidVideoSubFinderOCR:
     def __init__(self, vsf_exe_path: str = None, **ocr_params) -> None:
         if vsf_exe_path is None:
-            raise ValueError('vsf_exe_path must not be None.')
+            raise ValueError("vsf_exe_path must not be None.")
 
         self.vsf = VideoSubFinder(vsf_exe_path)
         self.video_ocr = RapidVideOCR(**ocr_params)
-        self.video_formats = ['.mp4', '.avi', '.mov', '.mkv']
+        self.video_formats = [".mp4", ".avi", ".mov", ".mkv"]
         self.logger = get_logger()
 
-    def __call__(self, video_path: str, output_dir: str = 'outputs'):
+    def __call__(self, video_path: str, output_dir: str = "outputs"):
         if Path(video_path).is_dir():
-            video_list = Path(video_path).rglob('*.*')
+            video_list = Path(video_path).rglob("*.*")
             video_list = [
                 v for v in video_list if v.suffix.lower() in self.video_formats
             ]
         else:
             video_list = [video_path]
 
         self.logger.info(
-            'Extracting subtitle images with VideoSubFinder (takes quite a long time) ...'
+            "Extracting subtitle images with VideoSubFinder (takes quite a long time) ..."
         )
         video_num = len(video_list)
         for i, one_video in enumerate(video_list):
             self.logger.info(
-                f'[{i+1}/{video_num}] Starting to extract {one_video} key frame'
+                f"[{i+1}/{video_num}] Starting to extract {one_video} key frame"
             )
             with tempfile.TemporaryDirectory() as tmp_dir:
                 try:
                     self.vsf(str(one_video), tmp_dir)
                 except Exception as e:
-                    self.logger.error(f'Extract {one_video} error, {e}, skip')
+                    self.logger.error(f"Extract {one_video} error, {e}, skip")
                     continue
 
-                self.logger.info(f'[{i+1}/{video_num}] Starting to run {one_video} ocr')
+                self.logger.info(f"[{i+1}/{video_num}] Starting to run {one_video} ocr")
 
-                rgb_dir = Path(tmp_dir) / 'RGBImages'
+                rgb_dir = Path(tmp_dir) / "RGBImages"
                 if not list(rgb_dir.iterdir()):
                     self.logger.warning(
-                        f'Extracting frames from {one_video} is 0, skip'
+                        f"Extracting frames from {one_video} is 0, skip"
                     )
                     continue
 
                 save_name = Path(one_video).stem
                 save_srt_dir = Path(output_dir) / save_name
                 self.video_ocr(rgb_dir, save_srt_dir, save_name=save_name)
 
 
 def main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        '-vsf',
-        '--vsf_exe_path',
+        "-vsf",
+        "--vsf_exe_path",
         type=str,
         default=None,
-        help='The full path of VideoSubFinderWXW.exe.',
+        help="The full path of VideoSubFinderWXW.exe.",
     )
     parser.add_argument(
-        '-video_dir',
-        '--video_dir',
+        "-video_dir",
+        "--video_dir",
         type=str,
         default=None,
-        help='The full path of video or the path of video directory.',
+        help="The full path of video or the path of video directory.",
     )
     parser.add_argument(
-        '-i',
-        '--img_dir',
+        "-i",
+        "--img_dir",
         type=str,
         default=None,
-        help='The full path of RGBImages or TXTImages.',
+        help="The full path of RGBImages or TXTImages.",
     )
     parser.add_argument(
-        '-s',
-        '--save_dir',
+        "-s",
+        "--save_dir",
         type=str,
-        default='outputs',
+        default="outputs",
         help='The path of saving the recognition result. Default is "outputs" under the current directory.',
     )
     parser.add_argument(
-        '-o',
-        '--out_format',
+        "-o",
+        "--out_format",
         type=str,
-        default='all',
-        choices=['srt', 'txt', 'all'],
+        default="all",
+        choices=["srt", "txt", "all"],
         help='Output file format. Default is "all".',
     )
     parser.add_argument(
-        '-m',
-        '--mode',
+        "-m",
+        "--mode",
         type=str,
-        default='single',
-        choices=['single', 'concat'],
+        default="single",
+        choices=["single", "concat"],
         help='Which mode to run (concat recognition or single recognition). Default is "single".',
     )
     parser.add_argument(
-        '-b',
-        '--concat_batch',
+        "-b",
+        "--concat_batch",
         type=int,
         default=10,
-        help='The batch of concating image nums in concat recognition mode. Default is 10.',
+        help="The batch of concating image nums in concat recognition mode. Default is 10.",
     )
     parser.add_argument(
-        '-p',
-        '--print_console',
+        "-p",
+        "--print_console",
         type=bool,
         default=0,
         choices=[0, 1],
-        help='Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.',
+        help="Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.",
     )
     args = parser.parse_args()
 
-    is_concat_rec = 'concat' in args.mode
+    is_concat_rec = "concat" in args.mode
 
     if not (args.vsf_exe_path is None and args.video_dir is None):
         raise ValueError(
-            '--vsf_exe_path or --video_dir must not be None at the same time.'
+            "--vsf_exe_path or --video_dir must not be None at the same time."
         )
 
     if args.vsf_exe_path and args.video_dir:
         extractor = RapidVideoSubFinderOCR(
             vsf_exe_path=args.vsf_exe_path,
             is_concat_rec=is_concat_rec,
             concat_batch=args.concat_batch,
@@ -144,9 +144,9 @@
             concat_batch=args.concat_batch,
             out_format=args.out_format,
             is_print_console=args.print_console,
         )
         extractor(args.img_dir, args.save_dir)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## rapid_videocr/rapid_videocr.py

```diff
@@ -1,31 +1,37 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 from pathlib import Path
-from typing import List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 from rapidocr_onnxruntime import RapidOCR
 from tqdm import tqdm
 
-from .utils import CropByProject, get_logger, mkdir
+from .utils import (
+    CropByProject,
+    compute_poly_iou,
+    get_logger,
+    is_inclusive_each_other,
+    mkdir,
+)
 
 CUR_DIR = Path(__file__).resolve().parent
 logger = get_logger()
 
 
 class RapidVideOCR:
     def __init__(
         self,
         is_concat_rec: bool = False,
         concat_batch: int = 10,
-        out_format: str = 'all',
+        out_format: str = "all",
         is_print_console: bool = False,
     ) -> None:
         """Init
 
         Args:
             is_concat_rec (bool, optional): Whether to single recognition. Defaults to False.
             concat_batch (int, optional): The batch of concating image nums in concat recognition mode. Defaults to 10.
@@ -40,187 +46,198 @@
         self.out_format = out_format
         self.is_print_console = is_print_console
 
     def __call__(
         self,
         video_sub_finder_dir: Union[str, Path],
         save_dir: Union[str, Path],
-        save_name: str = 'result',
+        save_name: str = "result",
     ) -> None:
         """call
 
         Args:
             video_sub_finder_dir (Union[str, Path]): RGBImages or TXTImages from VideoSubFinder app.
             save_dir (Union[str, Path]): The directory of saving the srt/txt file.
 
         Raises:
             RapidVideOCRError: meet some error.
         """
         video_sub_finder_dir = Path(video_sub_finder_dir)
         if not video_sub_finder_dir.exists():
-            raise RapidVideOCRError(f'{video_sub_finder_dir} does not exist.')
+            raise RapidVideOCRError(f"{video_sub_finder_dir} does not exist.")
 
         dir_name = Path(video_sub_finder_dir).name
-        is_txt_dir = 'TXTImages' in dir_name
+        is_txt_dir = "TXTImages" in dir_name
 
         save_dir = Path(save_dir)
         mkdir(save_dir)
 
-        img_list = list(Path(video_sub_finder_dir).glob('*.jpeg'))
+        img_list = list(Path(video_sub_finder_dir).glob("*.jpeg"))
         img_list = sorted(img_list, key=self.get_sort_key)
         if not img_list:
             raise RapidVideOCRError(
-                f'{video_sub_finder_dir} has not images with jpeg as suffix.'
+                f"{video_sub_finder_dir} has not images with jpeg as suffix."
             )
 
         if self.is_concat_rec:
-            logger.info('[OCR] Running with concat recognition.')
+            logger.info("[OCR] Running with concat recognition.")
             srt_result, txt_result = self.concat_rec(img_list, is_txt_dir)
         else:
-            logger.info('[OCR] Running with single recognition.')
+            logger.info("[OCR] Running with single recognition.")
             srt_result, txt_result = self.single_rec(img_list)
 
         self.export_file(save_dir, save_name, srt_result, txt_result)
 
         if self.is_print_console:
             self.print_console(txt_result)
 
     @staticmethod
-    def get_sort_key(x):
-        return int(''.join(str(x.stem).split('_')[:4]))
+    def get_sort_key(x: Path) -> int:
+        return int("".join(str(x.stem).split("_")[:4]))
 
-    def single_rec(self, img_list: List[str]) -> Tuple[List, List]:
+    def single_rec(self, img_list: List[Path]) -> Tuple[List[str], List[str]]:
         srt_result, txt_result = [], []
-        for i, img_path in enumerate(tqdm(img_list, desc='OCR')):
+        for i, img_path in enumerate(tqdm(img_list, desc="OCR")):
             time_str = self.get_time(img_path)
 
             img = cv2.imdecode(np.fromfile(img_path, dtype=np.uint8), 1)
             img = self.padding_img(img, (img.shape[0], img.shape[0], 0, 0))
             dt_boxes, rec_res = self.run_ocr(img)
             if rec_res:
                 txts = self.process_same_line(dt_boxes, rec_res)
-                srt_result.append(f'{i+1}\n{time_str}\n{txts}\n')
-                txt_result.append(f'{txts}\n')
+            else:
+                txts = ""
+
+            srt_result.append(f"{i+1}\n{time_str}\n{txts}\n")
+            txt_result.append(f"{txts}\n")
         return srt_result, txt_result
 
-    def concat_rec(
-        self, img_list: List[np.ndarray], is_txt_dir: bool
-    ) -> Tuple[List, List]:
+    def concat_rec(self, img_list: List[Path], is_txt_dir: bool) -> Tuple[List, List]:
         srt_result, txt_result = [], []
 
         img_nums = len(img_list)
-        for start_i in tqdm(range(0, img_nums, self.batch_size), desc='OCR'):
+        for start_i in tqdm(range(0, img_nums, self.batch_size), desc="OCR"):
             end_i = min(img_nums, start_i + self.batch_size)
 
             concat_img, img_coordinates, img_paths = self.get_batch(
                 img_list, start_i, end_i, is_txt_dir
             )
             dt_boxes, rec_res = self.run_ocr(concat_img)
-            if not rec_res:
+            if rec_res is None or dt_boxes is None:
                 continue
 
             srt_part, txt_part = self.get_match_results(
                 start_i, img_coordinates, dt_boxes, rec_res, img_paths
             )
             srt_result.extend(srt_part)
             txt_result.extend(txt_part)
         return srt_result, txt_result
 
     def get_batch(
-        self, img_list: List[str], start: int, end: int, is_txt_dir: bool
-    ) -> Tuple[np.ndarray, np.ndarray, List]:
+        self, img_list: List[Path], start: int, end: int, is_txt_dir: bool
+    ) -> Tuple[np.ndarray, np.ndarray, List[Path]]:
         select_imgs = img_list[start:end]
 
-        img_list, img_coordinates, batch_img_paths = [], [], []
+        padding_value = 10
+        array_img_list, img_coordinates, batch_img_paths = [], [], []
         for i, img_path in enumerate(select_imgs):
             batch_img_paths.append(img_path)
 
-            img = cv2.imread(str(img_path))
+            img = cv2.imdecode(np.fromfile(str(img_path), dtype=np.uint8), 1)
 
             if is_txt_dir:
                 img = cv2.resize(img, None, fx=0.25, fy=0.25)
 
-            img_list.append(img)
+            pad_img = self.padding_img(img, (0, padding_value, 0, 0))
+            array_img_list.append(pad_img)
 
             h, w = img.shape[:2]
-            img_coordinates.append([(0, i * h), (w, (i + 1) * h)])
+            x0, y0 = 0, i * (h + padding_value)
+            x1, y1 = w, (i + 1) * (h + padding_value)
+            img_coordinates.append([(x0, y0), (x1, y0), (x1, y1), (x0, y1)])
 
-        concat_img = np.vstack(img_list)
+        concat_img = np.vstack(array_img_list)
         return concat_img, np.array(img_coordinates), batch_img_paths
 
     def get_match_results(
         self,
         start_i: int,
         img_coordinates: np.ndarray,
         dt_boxes: np.ndarray,
-        rec_res: List,
-        img_paths: list,
-    ) -> Tuple[List, List]:
+        rec_res: Tuple[str],
+        img_paths: List[Path],
+    ) -> Tuple[List[str], List[str]]:
         srt_result_part, txt_result_part = [], []
 
-        match_dict = {}
-        y_points = img_coordinates[:, :, 1]
-        left_top_boxes = dt_boxes[:, 0, :]
-        for i, one_left in enumerate(left_top_boxes):
-            y = one_left[1]
-            condition = (y >= y_points[:, 0]) & (y < y_points[:, 1])
-            index = np.argwhere(condition)
-            if not index.size:
-                match_dict[i] = ''
-                continue
-
-            matched_index = index.squeeze().tolist()
-            matched_path = img_paths[matched_index]
-            match_dict.setdefault(matched_index, []).append(
-                [matched_path, dt_boxes[i], rec_res[i]]
-            )
+        match_dict: Dict[int, List[Union[Path, np.ndarray, str]]] = {
+            k: [] for k in range(len(img_coordinates))
+        }
+        visited_idx = []
+        for i, frame_boxes in enumerate(img_coordinates):
+            for idx, dt_box in enumerate(dt_boxes):
+                if idx in visited_idx:
+                    continue
+
+                box_iou = compute_poly_iou(frame_boxes, dt_box)
+                if is_inclusive_each_other(frame_boxes, dt_box) or box_iou > 0.1:
+                    matched_path = img_paths[idx]
+                    match_dict.setdefault(i, []).append(
+                        [matched_path, dt_box, rec_res[idx]]
+                    )
+                    visited_idx.append(idx)
 
         for k, v in match_dict.items():
             cur_frame_idx = start_i + k
-            img_path, boxes, recs = list(zip(*v))
+            if v:
+                img_path, boxes, recs = list(zip(*v))
+                time_str = self.get_time(img_path[0])
+                txts = self.process_same_line(boxes, recs)
+            else:
+                time_str = self.get_time(img_paths[k])
+                txts = ""
 
-            time_str = self.get_time(img_path[0])
-            txts = self.process_same_line(boxes, recs)
-            srt_result_part.append(f'{cur_frame_idx+1}\n{time_str}\n{txts}\n')
-            txt_result_part.append(f'{txts}\n')
+            srt_result_part.append(f"{cur_frame_idx+1}\n{time_str}\n{txts}\n")
+            txt_result_part.append(f"{txts}\n")
         return srt_result_part, txt_result_part
 
     @staticmethod
     def get_time(file_path: Path) -> str:
         """根据文件名称解析对应时间戳
 
         Args:
             file_path (Path): 字幕关键帧图像路径
 
         Returns:
             str: 字幕开始和截止时间戳字符串
         """
-        split_paths = file_path.stem.split('_')
+        split_paths = file_path.stem.split("_")
         start_time = split_paths[:4]
-        start_time[0] = f'{start_time[0]:0>2}'
-        start_str = ':'.join(start_time[:3]) + f',{start_time[3]}'
+        start_time[0] = f"{start_time[0]:0>2}"
+        start_str = ":".join(start_time[:3]) + f",{start_time[3]}"
 
         end_time = split_paths[5:9]
-        end_time[0] = f'{end_time[0]:0>2}'
-        end_str = ':'.join(end_time[:3]) + f',{end_time[3]}'
-        return f'{start_str} --> {end_str}'
-
-    def run_ocr(self, img: np.ndarray) -> Tuple[np.ndarray, List]:
+        end_time[0] = f"{end_time[0]:0>2}"
+        end_str = ":".join(end_time[:3]) + f",{end_time[3]}"
+        return f"{start_str} --> {end_str}"
+
+    def run_ocr(
+        self, img: np.ndarray
+    ) -> Tuple[Optional[np.ndarray], Optional[Tuple[str]]]:
         ocr_result, _ = self.rapid_ocr(img)
         if ocr_result is None:
             return None, None
 
         dt_boxes, rec_res, _ = list(zip(*ocr_result))
         return np.array(dt_boxes), rec_res
 
     @staticmethod
     def padding_img(
         img: np.ndarray,
         padding_value: Tuple[int, int, int, int],
-        padding_color: Tuple = (0, 0, 0),
+        padding_color: Tuple[int, int, int] = (0, 0, 0),
     ) -> np.ndarray:
         padded_img = cv2.copyMakeBorder(
             img,
             padding_value[0],
             padding_value[1],
             padding_value[2],
             padding_value[3],
@@ -243,61 +260,61 @@
         final_res, used = [], [False] * rec_len
         for is_same_line, pair_point in zip(bool_res, pair_points):
             if is_same_line:
                 concat_str = []
                 for v in pair_point:
                     used[v] = True
                     concat_str.append(rec_res[v])
-                final_res.append(' '.join(concat_str))
+                final_res.append(" ".join(concat_str))
             else:
                 for v in pair_point:
                     if not used[v]:
                         final_res.append(rec_res[v])
-        return '\n'.join(final_res)
+        return "\n".join(final_res)
 
     def export_file(
         self,
         save_dir: Union[str, Path],
         save_name: str,
         srt_result: List,
         txt_result: List,
     ) -> None:
         if isinstance(save_dir, str):
             save_dir = Path(save_dir)
 
-        srt_path = save_dir / f'{save_name}.srt'
-        txt_path = save_dir / f'{save_name}.txt'
+        srt_path = save_dir / f"{save_name}.srt"
+        txt_path = save_dir / f"{save_name}.txt"
 
-        if self.out_format == 'txt':
+        if self.out_format == "txt":
             self.save_file(txt_path, txt_result)
-        elif self.out_format == 'srt':
+        elif self.out_format == "srt":
             self.save_file(srt_path, srt_result)
-        elif self.out_format == 'all':
+        elif self.out_format == "all":
             self.save_file(txt_path, txt_result)
             self.save_file(srt_path, srt_result)
         else:
-            raise ValueError(f'The {self.out_format} dost not support.')
-        logger.info(f'[OCR] The result has been saved to {save_dir} directory.')
+            raise ValueError(f"The {self.out_format} dost not support.")
+        logger.info(f"[OCR] The result has been saved to {save_dir} directory.")
 
     def print_console(self, txt_result: List) -> None:
         for v in txt_result:
             print(v.strip())
 
     @staticmethod
-    def save_file(save_path: Union[str, Path], content: list, mode: str = 'w') -> None:
+    def save_file(save_path: Union[str, Path], content: List, mode: str = "w") -> None:
         if not isinstance(save_path, str):
             save_path = str(save_path)
 
         if not isinstance(content, list):
             content = [content]
 
-        with open(save_path, mode, encoding='utf-8') as f:
+        with open(save_path, mode, encoding="utf-8") as f:
             for value in content:
-                f.write(f'{value}\n')
-        logger.info(f'[OCR] The file has been saved in the {save_path}')
+                f.write(f"{value}\n")
+        logger.info(f"[OCR] The file has been saved in the {save_path}")
 
     @staticmethod
     def _compute_centroid(points: np.ndarray) -> List:
         """计算所给框的质心坐标
 
         :param points ([type]): (4, 2)
         :return: [description]
@@ -322,65 +339,65 @@
 class RapidVideOCRError(Exception):
     pass
 
 
 def main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument(
-        '-i',
-        '--img_dir',
+        "-i",
+        "--img_dir",
         type=str,
         required=True,
-        help='The full path of RGBImages or TXTImages.',
+        help="The full path of RGBImages or TXTImages.",
     )
     parser.add_argument(
-        '-s',
-        '--save_dir',
+        "-s",
+        "--save_dir",
         type=str,
-        default='outputs',
+        default="outputs",
         help='The path of saving the recognition result. Default is "outputs" under the current directory.',
     )
     parser.add_argument(
-        '-o',
-        '--out_format',
+        "-o",
+        "--out_format",
         type=str,
-        default='all',
-        choices=['srt', 'txt', 'all'],
+        default="all",
+        choices=["srt", "txt", "all"],
         help='Output file format. Default is "all".',
     )
     parser.add_argument(
-        '-m',
-        '--mode',
+        "-m",
+        "--mode",
         type=str,
-        default='single',
-        choices=['single', 'concat'],
+        default="single",
+        choices=["single", "concat"],
         help='Which mode to run (concat recognition or single recognition). Default is "single".',
     )
     parser.add_argument(
-        '-b',
-        '--concat_batch',
+        "-b",
+        "--concat_batch",
         type=int,
         default=10,
-        help='The batch of concating image nums in concat recognition mode. Default is 10.',
+        help="The batch of concating image nums in concat recognition mode. Default is 10.",
     )
     parser.add_argument(
-        '-p',
-        '--print_console',
+        "-p",
+        "--print_console",
         type=bool,
         default=0,
         choices=[0, 1],
-        help='Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.',
+        help="Whether to print the subtitle results to console. 1 means to print results to console. Default is 0.",
     )
     args = parser.parse_args()
 
-    is_concat_rec = 'concat' in args.mode
+    is_concat_rec = "concat" in args.mode
     extractor = RapidVideOCR(
         is_concat_rec=is_concat_rec,
         concat_batch=args.concat_batch,
         out_format=args.out_format,
         is_print_console=args.print_console,
     )
     extractor(args.img_dir, args.save_dir)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## rapid_videocr/utils.py

```diff
@@ -1,19 +1,21 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import functools
 import logging
 import sys
 from pathlib import Path
-from typing import List
+from typing import List, Union
 
 import colorlog
 import cv2
 import numpy as np
+import shapely
+from shapely.geometry import MultiPoint, Polygon
 
 logger_initialized = {}
 
 
 class CropByProject:
     """投影法裁剪"""
 
@@ -26,78 +28,143 @@
         # 将图片二值化
         retval, img = cv2.threshold(image, self.threshold, 255, cv2.THRESH_BINARY_INV)
 
         # 使文字增长成块
         closed = cv2.dilate(img, None, iterations=1)
 
         # 水平投影
-        x0, x1 = self.get_project_loc(closed, direction='width')
+        x0, x1 = self.get_project_loc(closed, direction="width")
 
         # 竖直投影
-        y0, y1 = self.get_project_loc(closed, direction='height')
+        y0, y1 = self.get_project_loc(closed, direction="height")
 
         return origin_img[y0:y1, x0:x1]
 
     @staticmethod
     def get_project_loc(img, direction):
         """获得裁剪的起始和终点索引位置
         Args:
             img (ndarray): 二值化后得到的图像
             direction (str): 'width/height'
         Raises:
             ValueError: 不支持的求和方向
         Returns:
             tuple: 起始索引位置
         """
-        if direction == 'width':
+        if direction == "width":
             axis = 0
-        elif direction == 'height':
+        elif direction == "height":
             axis = 1
         else:
-            raise ValueError(f'direction {direction} is not supported!')
+            raise ValueError(f"direction {direction} is not supported!")
 
         loc_sum = np.sum(img == 255, axis=axis)
         loc_range = np.argwhere(loc_sum > 0)
         i0, i1 = loc_range[0][0], loc_range[-1][0]
         return i0, i1
 
 
 def mkdir(dir_path):
     Path(dir_path).mkdir(parents=True, exist_ok=True)
 
 
-def read_txt(txt_path: str) -> List:
+def read_txt(txt_path: Union[str, Path]) -> List[str]:
     if not isinstance(txt_path, str):
         txt_path = str(txt_path)
 
-    with open(txt_path, 'r', encoding='utf-8') as f:
-        data = list(map(lambda x: x.rstrip('\n'), f))
+    with open(txt_path, "r", encoding="utf-8") as f:
+        data = list(map(lambda x: x.rstrip("\n"), f))
     return data
 
 
 @functools.lru_cache()
-def get_logger(name='rapid_videocr'):
+def get_logger(name="rapid_videocr"):
     logger = logging.getLogger(name)
     if name in logger_initialized:
         return logger
 
     for logger_name in logger_initialized:
         if name.startswith(logger_name):
             return logger
 
-    fmt_string = '%(log_color)s[%(asctime)s] [%(name)s] %(levelname)s: %(message)s'
+    fmt_string = "%(log_color)s[%(asctime)s] [%(name)s] %(levelname)s: %(message)s"
     log_colors = {
-        'DEBUG': 'white',
-        'INFO': 'white',
-        'WARNING': 'yellow',
-        'ERROR': 'red',
-        'CRITICAL': 'purple',
+        "DEBUG": "white",
+        "INFO": "white",
+        "WARNING": "yellow",
+        "ERROR": "red",
+        "CRITICAL": "purple",
     }
     fmt = colorlog.ColoredFormatter(fmt_string, log_colors=log_colors)
     stream_handler = logging.StreamHandler(stream=sys.stdout)
     stream_handler.setFormatter(fmt)
     logger.addHandler(stream_handler)
 
     logger.setLevel(logging.INFO)
     logger_initialized[name] = True
     logger.propagate = False
     return logger
+
+
+def compute_poly_iou(a: np.ndarray, b: np.ndarray) -> float:
+    """计算两个多边形的IOU
+
+    Args:
+        poly1 (np.ndarray): (4, 2)
+        poly2 (np.ndarray): (4, 2)
+
+    Returns:
+        float: iou
+    """
+    poly1 = Polygon(a).convex_hull
+    poly2 = Polygon(b).convex_hull
+
+    union_poly = np.concatenate((a, b))
+
+    if not poly1.intersects(poly2):
+        return 0.0
+
+    try:
+        inter_area = poly1.intersection(poly2).area
+        union_area = MultiPoint(union_poly).convex_hull.area
+    except shapely.geos.TopologicalError:
+        print("shapely.geos.TopologicalError occured, iou set to 0")
+        return 0.0
+
+    if union_area == 0:
+        return 0.0
+
+    return float(inter_area) / union_area
+
+
+def is_inclusive_each_other(box1: np.ndarray, box2: np.ndarray) -> bool:
+    """判断两个多边形框是否存在包含关系
+
+    Args:
+        box1 (np.ndarray): (4, 2)
+        box2 (np.ndarray): (4, 2)
+
+    Returns:
+        bool: 是否存在包含关系
+    """
+    poly1 = Polygon(box1)
+    poly2 = Polygon(box2)
+
+    poly1_area = poly1.convex_hull.area
+    poly2_area = poly2.convex_hull.area
+
+    if poly1_area > poly2_area:
+        box_max = box1
+        box_min = box2
+    else:
+        box_max = box2
+        box_min = box1
+
+    x0, y0 = np.min(box_min[:, 0]), np.min(box_min[:, 1])
+    x1, y1 = np.max(box_min[:, 0]), np.max(box_min[:, 1])
+
+    edge_x0, edge_y0 = np.min(box_max[:, 0]), np.min(box_max[:, 1])
+    edge_x1, edge_y1 = np.max(box_max[:, 0]), np.max(box_max[:, 1])
+
+    if x0 >= edge_x0 and y0 >= edge_y0 and x1 <= edge_x1 and y1 <= edge_y1:
+        return True
+    return False
```

## Comparing `rapid_videocr-2.2.1.dist-info/LICENSE` & `rapid_videocr-2.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapid_videocr-2.2.1.dist-info/METADATA` & `rapid_videocr-2.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-videocr
-Version: 2.2.1
+Version: 2.2.2
 Summary: Tool for extracting hard subtitles from videos.
 Home-page: https://github.com/SWHL/RapidVideOCR.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr,videocr,subtitle
 Platform: Any
@@ -45,16 +45,16 @@
 
 ### 2. Run by script.
 - Only OCR:
     ```python
     from rapid_videocr import RapidVideOCR
 
     extractor = RapidVideOCR(is_concat_rec=True,
-                            concat_batch=10,
-                            out_format='srt')
+                             concat_batch=10,
+                             out_format='srt')
 
     rgb_dir = 'RGBImages'
     save_dir = 'outputs'
     extractor(video_sub_finder_dir=rgb_dir, save_dir=save_dir)
     ```
 - Extract + OCR:
     ```python
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.1 Summary: Tool for
+Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.2 Summary: Tool for
 extracting hard subtitles from videos. Home-page: https://github.com/SWHL/
 RapidVideOCR.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: rapidocr,videocr,subtitle Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

## Comparing `rapid_videocr-2.2.1.dist-info/RECORD` & `rapid_videocr-2.2.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 rapid_videocr/__init__.py,sha256=eODelyqvjJaceBues-U7fmLAE3JTDkVLUTbcsWivf_Q,174
-rapid_videocr/main.py,sha256=e3v3-QeJcJ-FwNitLWG-rLcZzCGp2ghputjnOT4jp-A,4798
-rapid_videocr/rapid_videocr.py,sha256=0BB0FREm7_PN3r_V52aKzLHA0S7nEuad492NHfijl9o,12743
-rapid_videocr/utils.py,sha256=AWQvgtn8429FnVPYdixHNYEEB4gjJRgKl4aHEcTgzBk,2756
+rapid_videocr/main.py,sha256=SO9Lc40vDQw4p4gqN0JOuhkWNKCXJIPOTJS4so7KOkk,4798
+rapid_videocr/rapid_videocr.py,sha256=Ha-Llqez4nLof93d36aSyOlhiTzF7YECEbFrYwV5Jtg,13456
+rapid_videocr/utils.py,sha256=wyUh1Oy5h8X2odUWmzeqkZn9csUQaOymoOnBSMJEUKs,4479
 rapid_videocr/video_sub_finder.py,sha256=6TAfUM3pAWgzzn4xK6Ln2EB7XvWc4BTkz_LLUVu4vZ8,1264
-rapid_videocr-2.2.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-rapid_videocr-2.2.1.dist-info/METADATA,sha256=iH8RrZYnjQHxbx8Af_OsH4LSkj8Mu4vspA2JeXtc4X8,4648
-rapid_videocr-2.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-rapid_videocr-2.2.1.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
-rapid_videocr-2.2.1.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
-rapid_videocr-2.2.1.dist-info/RECORD,,
+rapid_videocr-2.2.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+rapid_videocr-2.2.2.dist-info/METADATA,sha256=FqetSUoc3oxF8zCNvPivVswx4BB78NRT-8MwrqtuwS8,4650
+rapid_videocr-2.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+rapid_videocr-2.2.2.dist-info/entry_points.txt,sha256=-keKc5D46wZRqKWIPVZqb5paoQwqLf-OiXKtztK9VqA,59
+rapid_videocr-2.2.2.dist-info/top_level.txt,sha256=uPQbJQ346YJVTUi4CqGP2OZUrUSsUn57eiRiNtpe97E,14
+rapid_videocr-2.2.2.dist-info/RECORD,,
```

