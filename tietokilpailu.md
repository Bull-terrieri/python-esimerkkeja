## Tietokilpailu (Quiz)

Tämä Python-koodi toteuttaa yksinkertaisen tietokilpailun, jossa käyttäjä vastaa kysymyksiin ja saa palautteen vastauksistaan. Koodi on tehty opetuskäyttöön ja havainnollistaa muun muassa syötteiden käsittelyä, ehtolauseita ja ohjelman loogista rakennetta.

Esimerkki soveltuu hyvin ohjelmoinnin perusteiden harjoitteluun ja jatkokehittämisen pohjaksi.

---

print("Tervetuloa tietokilpailuun!")
print("Vastaa seuraaviin kysymyksiin oikein voittaaksesi.")

score = 0  # Alustetaan pistemäärä

# Kysymykset
question1 = "Mikä on maailman suurin valtameri? "
question2 = "Mikä on pääkaupunki Suomessa? "
question3 = "Mikä on maailman eteläisin manner? "

# Oikeat vastaukset
answer1 = "Tyyni valtameri"
answer2 = "Helsinki"
answer3 = "Etelämanner"

# Kysytään ensimmäinen kysymys
guess1 = input(question1)
if guess1.capitalize() == answer1:
    print("Oikein!")
    score += 1
else:
    print("Väärin!")

# Kysytään toinen kysymys
guess2 = input(question2)
if guess2.capitalize() == answer2:
    print("Oikein!")
    score += 1
else:
    print("Väärin!")

# Kysytään kolmas kysymys
guess3 = input(question3)
if guess3.capitalize() == answer3:
    print("Oikein!")
    score += 1
else:
    print("Väärin!")

# Lopputuloksen tulostus
print("Pistemääräsi on:", score, "/ 3")

if score == 3:
    print("Onnittelut! Voitit tietokilpailun!")
else:
    print("Kiitos osallistumisesta.")
