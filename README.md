<center> <h1> Building Recommender System </h1> </center>

----

<div id="theory"><h2>Latar Belakang</h2><div class="p-Widget jp-Cell jp-MarkdownCell jp-mod-rendered jp-Notebook-cell jp-mod-active jp-mod-selected">
<div class="p-Widget p-Panel jp-Cell-inputWrapper">
<div class="p-Widget jp-InputArea jp-Cell-inputArea">
<div class="p-Widget jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p style="text-align: justify;">Terdapat 2 dasar tipe sistem rekomendasi:</p>
<ol style="text-align: justify;">
<li>Sistem Rekomendasi <strong>Sederhana</strong></li>
<li>Sistem Rekomendasi <strong>Berdasarkan Konten dari Fiturnya</strong></li>
</ol>
</div>
</div>
</div>
<div class="p-Widget jp-CellFooter jp-Cell-footer" style="text-align: justify;">&nbsp;</div>
</div>

Sistem Rekomendasi Sederhana</strong>, seperti namanya adalah sistem rekomendasi yang hanya <strong>menggunakan urutan sebagai dasar perhitungannya</strong>, yang biasanya digunakan dalam '5 film terbaik' kita akan menggunakan urutan berdasarkan mungkin vote terbanyak, rating tertinggi, penjualan film paling tinggi, atau apapun yang lain.</div>
<div class="p-Widget p-Panel jp-Cell-inputWrapper">
<div class="p-Widget jp-InputArea jp-Cell-inputArea">
<div class="p-Widget jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p style="text-align: justify;">Dalam kasus ini, kita akan menggunakan kombinasi antara rata-rata rating, jumlah vote, dan membentuk metric baru dari metric yang sudah ada, kemudian kita akan melakukan sorting untuk metric ini dari yang tertinggi ke terendah.</p>
</div>
</div>
</div>
</div></div>

<div id="theory"><h2>Simple Recommender Engine using Weighted Average</h2><p>Simple Recommender Engine menawarkan rekomendasi yang umum untuk semua user berdasarkan popularitas film dan terkadang genre.</p>
<p>Ide awal di balik sistem rekomendasi ini adalah sebagai berikut.</p>
<ol>
<li>Film-film yang lebih populer akan memiliki kemungkinan yang lebih besar untuk disukai juga oleh rata-rata penonton.</li>
<li>Model ini tidak memberikan rekomendasi yang personal untuk setiap tipe user.&nbsp;</li>
<li>Implementasi model ini pun juga bisa dibilang cukup mudah, yang perlu kita lakukan hanyalah mengurutkan film-film tersebut berdasarkan rating dan popularitas dan menunjukkan film teratas dari list film tersebut.</li>
</ol>
<p>Sebagai tambahan, kita dapat menambahkan genre untuk mendapatkan film teratas untuk genre spesifik tersebut</p></div>

<h2>Formula dari IMDB dengan Weighted Rating</h2><p>&nbsp;</p>  
    
![](formula.png)  
    
<p>dimana,</p>
<p>v: jumlah votes untuk film tersebut<br>m: jumlah minimum votes yang dibutuhkan supaya dapat masuk dalam chart<br>R: rata-rata rating dari film tersebut<br>C: rata-rata jumlah votes dari seluruh semesta film</p></div>

----

![](certificate.jpg)