# dask-image: distributed image processing for large data

A talk presented by Genevieve Buckley, 2020

* [Watch it at PyConlineAU 2020](https://www.youtube.com/watch?v=MpjgzNeISeI&list=PLs4CJRBY5F1IEFq-wumrBDRCu2EqkpY-R&index=2) (presentation in English only)
* [Watch it at SciPy Japan 2020](https://www.youtube.com/watch?v=dP0m2iZX0PU) (presentation in English, captions in Japanese)
* [See the talk slides](https://genevievebuckley.github.io/dask-image-talk-2020/)

This talk introduces dask-image, a python library for distributed image processing. Targeted towards applications involving large array data too big to fit in memory, dask-image is built on top of numpy, scipy, and dask allowing easy scalability and portability from your laptop to the supercomputing cluster. It is of broad interest to a diverse range of scientific fields including astronomy, geosciences, microscopy, and climate sciences. We will provide a general overview of the dask-image library, then discuss mixing and matching with your own custom functions, and present a practical case study of a python image processing pipeline.

この講演では、分散画像処理のための python ライブラリである dask-image を紹介します。メモリに収まりきらないほど大きな配列データを扱うアプリケーションをターゲットにしており、dask-image は numpy, scipy, dask の上に構築されているため、ラップトップからスーパーコンピュータクラスタへの拡張性と移植性を容易にします。天文学、地球科学、顕微鏡、気候科学などの多様な科学分野に広く関心があります。dask-image ライブラリの一般的な概要を説明した後、独自のカスタム関数との混合やマッチングについて議論し、Python 画像処理パイプラインの実践的なケーススタディを紹介します。
