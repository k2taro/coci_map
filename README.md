# coci_map
[COCI(the OpenCitations Index of Crossref open DOI-to-DOI citations)](https://opencitations.net/index/coci)で作る共引用マップ。  
詳細な手法の説明やクラスタリング結果、マッピング結果についての詳細な分析は今後の宿題。

# Poster
とある場所で発表した[ポスター](https://github.com/k2taro/coci_map/blob/master/coci_public.pdf)

# HTML版マップ
[coci_map.html](https://github.com/k2taro/coci_map/blob/master/coci_map.html)
[githubpagesの単独動作版](https://k2taro.github.io/coci_map.html)


# クラスタリング結果・マップのデータ
・[core_paper_final_pub.csv](https://github.com/k2taro/coci_map/blob/master/core_paper_final_pub.csv)  
論文の書誌情報・クラスタリング結果  
- DOI_COCI : DOI from COCI  
- #cited : Number of cited paper from the window(2015-2017)  
- title_crossref : Paper title from crossref API  
- journal_crossref : Journal title from crossref API  
- ISSN_crossref : Journal's ISSN from crossref API  
- sourceid_SCIMago : Sourceid of SCIMago  
- cls_final : Clustering result  
  

・[cls_final_pub.csv](https://github.com/k2taro/coci_map/blob/master/cls_final_pub.csv)  
クラスタリング結果の分野・マップ上の位置  
- cls_final : Cluster name  
- subject_name : Subject of cluster(from SCIMago journal list)  
- V1 : X axis of the map(NA:Cannot calcurate position because the cluster has no co-citation edge to another cluster)  
- V2 : Y axis of the map(NA:Cannot calcurate position because the cluster hos no co-citation edge to another cluster)  



# Data source  
・COCI 2018年12月ダンプデータ  
　445,826,118：citations(引用の数)  
　46,534,705：bibliographic resources(含まれる論文数)  
　https://doi.org/10.6084/m9.figshare.6741422.v3

・Crossref REST API  
　https://www.crossref.org/services/metadata-delivery/rest-api/

・SCIMago ジャーナルリスト  
  http://www.scimagojr.com (Retrieved 2019-12-20)
