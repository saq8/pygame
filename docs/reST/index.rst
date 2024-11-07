import pygame
import sys

# Initialize Pygame
pygame.init()

# Set up display
width, height = 800, 600
screen = pygame.display.set_mode((width, height))
pygame.display.set_caption("Move the Red Square")

# Set up colors
RED = (255, 0, 0)
WHITE = (255, 255, 255)

# Set up player (a simple red square)
player_size = 50
player_x, player_y = width // 2, height // 2
player_speed = 5

# Set up clock for controlling FPS
clock = pygame.time.Clock()

# Game loop
while True:
    # Handle events (keyboard, close window)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    # Handle movement (arrow keys)
    keys = pygame.key.get_p
