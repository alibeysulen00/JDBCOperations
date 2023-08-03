<h1> JDBC Nedir ? </h1>
<i>
<p> Java ile veritabanı sistemleri arasındaki iletişim JDBC( Java Database Connectivity) isimli bir API aracılığıyla gerçekleştirilir. JDBC veritabanı sistemlerine bağlanarak SQL sorguları gönderir. Böylelikle veritabanı üzerinde çeşitli işlemlerin gerçekleştirilmesini ve aynı zamanda gönderilen sorgulardan elde edilen verilerin Java ya getirilmesini sağlar
</i>




<h2>Bir JDBC uygulaması oluşturmak için Temel adımlar nelerdir ?  </h2>

<ol>
<li> Veritabanı programlama için gereken <b>JDBC</b> sınıflarını içeren paketleri içe aktarın  </li>
<li> Veritabanıyla bir iletişim kanalı açabilmeniz için<b> JDBC </b>sürücüsünü kaydedin  </li>
<li><b> DriverManager.getConnection( )</b> yöntemini kullanarak bir bağlantı açın  </li>
<li> Açıklama türünde bir nesne kullanarak bir sorgu yürütün  </li>
<li> Uygun <b> ResultSet.getXXX ( )</b> yöntemini kullanarak sonuç kümesinden verileri çıkarın  </li>
<li><b> JVM</b> nin çöp toplamasına bağlı olarak tüm veritabanı kaynaklarını kapatarak ortamı temizleyin  </li>

</ol>




<h2>JDBC DriverManager Nedir ? </h2>
<p>Veritabanı sürücülerinin listesini yöneten bir sınıftır. Java uygulamasından gelen bağlantı isteklerini iletişim alt protokolünü kullanarak uygun veritabanı sürücüsüyle eşleştirir.

<h2>JDBC Driver nedir?  </h2>
<p>JDBC  Driver, bir java uygulamasının bir veritabanıyla etkileşime girmesini sağlayan bir arabirimdir. Bireysel veritabanlarıyla bağlantı kurmak için JDBC her veritabanı için sürücüler gerektirir. JDBC sürücüsü veritabanı bağlantısını verir ve istemci ile veritabanı arasında sorgu ve sonucun aktarılması için protokolü uygular
<h2>JDBC Connection nedir ?  </h2>
<p>Bağlantı arayüzü, bir veritabanıyla iletişim kurma yöntemlerinden oluşur. Bağlantı nesnesi iletişim bağlamını temsil eder

<h2>Statment nedir ?   </h2>
<p>Statment, ayrıştırılmak, derlenmek, planlanmak ve yürütülmek üzere veritabanına aktarılan SQL ifadesini kapsüller


<h2>Bazı SQL komutları</h2>


<ul>
<li><b>Database oluşturma   </b><pre>    CREATE DATABASE db_name;   </li> 
<li> <b> Tablo oluşturma   </b><pre> 
CREATE TABLE table_name (
        id INTEGER NOT NULL,
        first_name VARCHAR(30),
        last_name VARCHAR(30),
        age INTEGER,
        PRIMARY KEY (id)

);

</pre>
                      </li> 
<li> <b>Tabloya Ekleme Yapma  </b> <pre> 
        INSERT INTO table_name (first_name, last_name,age) 
        VALUES ('Muhammet Ali', 'Beysülen', 22 );

  </li> 


</ul>



