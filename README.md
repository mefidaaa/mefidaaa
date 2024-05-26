#include <SFML/Graphics.hpp>

const int WIDTH = 10;
const int HEIGHT = 20;
bool field[WIDTH][HEIGHT] = {false};
int score = 0;

bool isCollision(int shape[4][4], int x, int y) {
    // Реалізація функції перевірки зіткнення
}

void mergeShape(int shape[4][4], int x, int y) {
    // Реалізація функції об'єднання фігур
}

void addScore(int rowsCleared) {
    // Реалізація функції підрахунку очок
}

bool checkGameOver() {
    // Реалізація функції перевірки завершення гри
}

int main() {
    sf::RenderWindow window(sf::VideoMode(400, 800), "Tetris");

    while (window.isOpen()) {
        sf::Event event;
        while (window.pollEvent(event)) {
            if (event.type == sf::Event::Closed)
                window.close();
        }

        window.clear(sf::Color::Black);

        // Відображення поля гри
        // TODO: Відобразити фігури тетріса та інше

        window.display();
    }

    return 0;
}
