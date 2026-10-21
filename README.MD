# ROS 2 Sıcaklık İzleyici Paketi

Bu paket, 20-40 arası rastgele sıcaklık değerleri üreten bir sensör düğümü ve bu değerleri dinleyip 30 derecenin üzerindeyse uyarı veren bir izleyici düğümü içerir.

## Çalıştırma Adımları

1. Çalışma alanınıza gidilir: cd ~/ros2_ws
   Paket derlernir: colcon build --packages-select sicaklik_izleyici_py

2. Sensör düğümü 1. terminalde çalıştırılır: source install/setup.bash
                                             ros2 run sicaklik_izleyici_py sensor

3. İzleyici düğümü 2. terminalde çalıştırılır: cd ~/ros2_ws
                                               source install/setup.bash
                                               ros2 run sicaklik_izleyici_py izleyici

4. Üçüncü terminalde iletişim ağı görüntülenir: rqt_graph
