class Brawler:
    def __init__(self, name, hp, power):
        self.hp = hp
        self.power = power
        self.name = name
    def attack(self, brawler):
        brawler.hp = brawler.hp - self.power
        if self.hp <= 0:
            print(self.name, 'умер')
        else:
            print(self.name, 'атаковал', brawler.name, 'у', brawler.name, 'осталось', brawler.hp, 'здоровья')
    def fight(self, brawler):
        while self.hp > 0 and brawler.hp > 0:
            if brawler.hp > 0:
                self.attack(brawler)
            if self.hp > 0:
                brawler.attack(self)
        if brawler.hp <= 0:
            print(self.name, 'победил')
        else:
            print(brawler.name, 'победил')
    def heal(self, i):
        self.hp += i
