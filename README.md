# jack-runner
Идея: упровляй кубиком и выживай

В игре есть три вида стен

- Стены которые нужно перепрыгивать
  
![](/img/screen_2.png)

- Стены под которыми нужно проезжать
 
![](/img/screen_3.png)

- Стены которые нужно обходить
  
![](/img/screen_4.png)

### Мы гордимся
- Генерацией сида пользователем
  
![](/img/screen_1.png)

- Обработкой столкновений, с помощью коллайдера
  
  ```
     method boolean isCollided(RectangleCollider collider) {
      if ((y > (collider.getY() + collider.getSizeY())) | ((y + sizeY) < collider.getY()))
      {
        return false;
      } 
      if ((x > (collider.getX() + collider.getSizeX())) | ((x + sizeX) < collider.getX()))
      {
        return false;
      } 
      return true;
   }
  ```
- Троллфейсом (Бобаном) 32х32 = смердженный 4х(16х16)
- Арбузом SimpleWall для проверок коллизии с любой стеной одним методом
