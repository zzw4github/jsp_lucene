To build the Apache Lucene web app demo just run 
"ant war-demo" from the Apache Lucene Installation
directory (follow the master instructions in 
BUILD.txt).  If you have questions please post 
them to the Apache Lucene mailing lists.  To 
actually figure this out you really need to 
read the Lucene "Getting Started" guide provided
with the doc build ("ant docs").




IndexFiles.java  在主目录下生成index文件夹，存放生成的文件，运行IndexFiles.java 的参数是要添加到索引的文件夹，如果是个文件夹，文件夹下的所有文件都会索引到
如果是哥文件，只有这个文件能被索引。
result.jsp 的61行
          IndexReader reader = IndexReader.open(FSDirectory.open(new File("f:\\workspace\\jsp_lucene\\index")), true);
"f:\\workspace\\jsp_lucene\\index" 是lucene生成的文件存放的位置。
