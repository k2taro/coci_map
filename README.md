# coci_map
[COCI(the OpenCitations Index of Crossref open DOI-to-DOI citations)](https://opencitations.net/index/coci)で作る共引用マップ。  
詳細な手法の説明やクラスタリング結果、マッピング結果についての詳細な分析は今後の宿題。

# Poster
とある場所で発表した[ポスター](https://github.com/k2taro/coci_map/blob/master/coci_public.pdf)

# HTML版マップ
[coci_map.html](https://k2taro.github.io/coci_map.html)

# マップされた論文(最終的なクラスタリング結果)
[core_paper_final.csv](https://github.com/k2taro/coci_map/blob/master/core_paper_final.csv)

# Data source  
・COCI 2018年12月ダンプデータ  
　445,826,118：citations(引用の数)  
　46,534,705：bibliographic resources(含まれる論文数)  
　https://doi.org/10.6084/m9.figshare.6741422.v3

・Crossref REST API  
　https://www.crossref.org/services/metadata-delivery/rest-api/

・SCIMago ジャーナルリスト  
  http://www.scimagojr.com (Retrieved 2019-12-20)
