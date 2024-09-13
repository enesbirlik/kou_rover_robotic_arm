# kou_rover_robotic_arm
# Bu yazı 2024-2025 Mekatronik Mühensiliği bitirme projesinde yapmak istediklerimi ve projenin genel sınırlarını tanıtır.

Merhaba ben Enes, KOU ROVER takımında 3 yıldır mobil robotlar ve AGV ler üzerine çalışıyorum. Geçtiğmiz yıllarda ROS ve ROS2 ile çeşitli çalışmalar yaptım. Görüntü işleme, lidar haritalandırması, robot kontrol algortimaları, robot ana görev algoritması vb gibi çeşitli alanlarda ekibimiz ile birlikte çalıştım. [KOU ROVER](https://www.linkedin.com/company/kou-rover/) takımı olarak bu yıl [European Rover Challange](https://roverchallenge.eu/) ve [Anatolian Rover Challange](https://www.anatolianrover.space/) yarışmalarına hazırlanmayı ve ülkemizi o yarışmalarda temsil etmeyi hedefliyoruz.


<img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/team_logo.png"  width="400"> <img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/ERC_logo.png"  width="200" > <img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/ARC_logo.png"  width="200">

## Bu yıl bitirme projesi olarak yapmak istediğim projenin aynı zamanda KOU ROVER takımında da kullanılacak bir robot kol olmasını planlıyorum. Bu robot kolun modüler bir yapıya sahip olmasını ve roverdan bağımsız çalışabilir bir halde olmasını istiyorum. Gerektiği zaman gezegen gezgini rover aracının mobil robot gövdesinin üzerine montelenerek çeşitli görevleri gerçekleştirmesini istiyorum. 

<img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/robotic_arm_example1.jpeg" alt="örnek robot kol 1" width="400"> <img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/robotic_arm_example2.jpg" alt="örnek robot kol 2"  width="400">

<img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/robotic_arm_example3.jpg" alt="örnek robot kol 3" width="400"> <img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/robotic_arm_example4.jpg" alt="örnek robot kol 4" width="400">

<img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/robotic_arm_example5.jpg" alt="örnek robot kol 5" width="400"> <img src="https://github.com/enesbirlik/kou_rover_robotic_arm/blob/main/robotic_arm_example6.jpg" alt="örnek robot kol 6" width="400">
# Projede yapmak istediğim robot kol resimdeki robot kollara benzer bir yapıda olacaktır.

Robot kol mekaniği ile ilgili pek bilgi sahibi değilim bu yüzden burayı pas geçiyorum şimdilik. (bu alanda olan çalışmalar bitirme projesi grubu ile ve KOU ROVER mekanik ekibi ile ortak yürütülebilir)
Motor seçimi malzeme seçimi vs yapıldıktan sonra malzemelerin edinilmesi gibi şeyler KOU ROVER organizasyon ekibi ile ortaklaşa yürütülerek sağlanmılması hedeflenmektedir.

Robot kolun enkoder vb çeşitli sensör verisini ROS2 ağına aktarması ve aynı şekilde ROS2 ağındaki hesaplamalara göre robot kolun aktüatörlerinin hareketinin sağlanması için gömülü elektronik tarafta şuan ön gördğüm 2 yol var.

birinci yol [microROS](https://micro.ros.org/docs/overview/features/) kullanarak gömülü yazılım kısmını ROS2 ekosistemine doğrudan entegre etmek (bu taraf zorlayıcı unsurlar içerir)(detay eklenecek daha sonra) https://micro.ros.org/docs/overview/hardware/
ikinci yol belirlenen X bir mikrodenetleyici kart ile çalışmalara devam edilir ve seri haberleşme ile ROS2 ağına veri gönderme işlemi gerçekleştirilir.


Robotun otonom ve kontrol yazılımları ise en kapsamlı süreç olacaktır. ros2_control paketi kullanarak kendi üreteceğimiz robotun modellenmesi ile gazebo simülasyon ortamında robotun yazılımlarının testleri daha erken bi süreçte başlayacaktır. Robot kol, roverın mobil robot gövdesi ile beraber hareket edeceği için çeşitli görev ve senaryolarara göre özel kabiliyetlere sahip olması gerekmektedir.


Robot kolun tasarım, üretim, test ve geliştirmeleri yapılırken tüm ekip aynı zamanda yarışma için gereken eleme raporlarında da görev alacaklardır. Bu raporlama ingilizce bir şekilde teknik döküman oluşturularak yapılmaktadır. Bu raporlamaları yaparken bir yandan da edindiğimiz tecrbeler ile bir akademik dergide de yayın yapabilmemiz iyi gien çalışmalarımız sonucunda mümkün gözükmektedir.
