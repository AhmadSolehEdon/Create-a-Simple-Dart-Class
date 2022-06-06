# Create-a-Simple-Dart-Class

![image](https://user-images.githubusercontent.com/106972846/172168947-450720e6-9f5f-427b-b482-ee61f43c970d.png)

class Bicycle {
  int cadence;
  int gear;
  int _speed = 0;
  
  int get speed => _speed;
  
  Bicycle(this.cadence, this.gear);

  void applyBrake(int decrement) {
  _speed -= decrement;
}

void speedUp(int increment) {
  _speed += increment;
}
  @override
String toString() => 'Bicycle: $_speed mph';
}

void main() {
   var bike = Bicycle(2, 1);
  print(bike);
}
