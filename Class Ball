class Ball {
  float x, y;
  float vx, vy;
  float radius;

  Ball() {
    x = random(width);
    y = random(height);
    radius = 10;
    vx = 3;
    vy = 2;
  }

  void draw() {
    ellipse(x, y, radius*2, radius*2);
  }

  void move() {
    x = x + vx;
    y = y + vy;
    if (x < radius || x > width-radius) {
      vx = -vx;
    }
    if (y < radius || y > height-radius) {
      vy = -vy;
    }
  }
}

Ball b;

void setup() {
  size(500, 500);

  b = new Ball();
}

void draw() {
  background(255);

  b.draw();
  b.move();
}
