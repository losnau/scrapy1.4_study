# scrapy1.4_study
study for scapy 1.4

### for my_exporters.py
1. 安装openpyxl 、xlwt库
2. 将my_exporters.py 放在项目与settings.py同级的目录下面
3. 编辑settings.py文件
``` python
FEED_EXPORTERS={'excel':'mayun.my_exporters.ExcelItemExporter','excel2':'mayun.my_exporters.ExcelItemExporter2'}
```
4. 运行
``` shell
#导出为xlsx文件
scrapy crawl pygists -t excel -o pygists.xlsx
#导出为xls文件
scrapy crawl pygists -t excel2 -o pygists.xls
```
