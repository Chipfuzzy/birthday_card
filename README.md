import pygame,sys
import time
from pygame.locals import QUIT

pygame.init() #initialises program

HEIGHT = 600
WIDTH = 600

display_surface=pygame.display.set_mode((600,600)) #creating dimensions
pygame.display.set_caption("birthday greeting card") #creating title

img=pygame.image.load("birthday1.jpg") #importing image
image = pygame.transform.scale(img, (WIDTH,HEIGHT)) #forming image size


while(True):
    display_surface.fill((255,255,255)) #creates screen color
    display_surface.blit(image,(0,0)) #initialising image
    pygame.display.update
    time.sleep(2)

    image2=pygame.image.load("b'day 2.jpg")
    display_surface.fill((255,255,255)) 
    display_surface.blit(image2,(0,0)) 
    pygame.display.update
    time.sleep(2)

    image3=pygame.image.load("b'day 3.jpg")
    display_surface.fill((255,255,255)) 
    display_surface.blit(image3,(0,0)) 
    pygame.display.update
    time.sleep(2)

    image4=pygame.image.load("b'day 4.jpg")
    display_surface.fill((255,255,255)) 
    display_surface.blit(image4,(0,0)) 
    pygame.display.update
    time.sleep(2)

    image5=pygame.image.load("b'day 5.jpg")
    display_surface.fill((255,255,255)) 
    display_surface.blit(image5,(0,0)) 
    pygame.display.update
    time.sleep(2)

    image6=pygame.image.load("b'day 6.jpg")
    display_surface.fill((255,255,255)) 
    display_surface.blit(image6,(0,0)) 
    pygame.display.update
    time.sleep(2)

    image7=pygame.image.load("b'day 7.jpg")
    display_surface.fill((255,255,255)) 
    display_surface.blit(image7,(0,0)) 
    pygame.display.update
    time.sleep(2)

    for event in pygame.event.get():
        if event.type == QUIT:
            pygame.quit()
            sys.exit()
    pygame.display.update()
