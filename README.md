# Fraction-addind-calculator
#Adds two fractions
def suurimnimetaja(Anim, Bnim):
    if Anim != Bnim:
        korrutamine = Anim * Bnim
    elif Anim == Bnim:
        vastuse_nimetaja = Anim
    return vastuse_nimetaja
def liitmine(tu, tv):
    if Anim != Bnim:
        vastuse_lugeja = tu * Bnim + tv * Anim
    elif Anim == Bnim:
        vastuse_lugeja = tu + tv
    return vastuse_lugeja
def kuvamurd (a, b):
    if a>b:
        return len(str(a)) * '-'
    else:
        return len(str(b)) * '-'

Alug = int(input("Sisesta arvu A lugeja: "))
Anim = int(input("Sisesta arvu A nimetaja: "))
Blug = int(input("Sisesta arvu B lugeja: "))
Bnim = int(input("Sisesta arvu B nimetaja: "))
nimetaja = suurimnimetaja(Anim, Bnim)
lugeja = liitmine(Alug, Blug)

print("""
%i   %i   %i
%s + %s = %s
%i   %i   %i
""" % (Alug, Blug, lugeja , kuvamurd(Alug, Anim), kuvamurd(Blug, Bnim), kuvamurd(lugeja, nimetaja), Anim, Bnim, nimetaja))
