# Trump - Twitter - Bot
Please do not take this so serious - This twitter Bot generates funny tweets. 
It was part of a python training. 


First I copied some of tweet parts and put them into lists

    part1 = ["Putin,", "Hillary,", "Obama", "Fake News,", "Mexico,", "Arnold Schwarzenegger", "The Democrats"]
    part2 = ["no talent,", "on the way down,", "really poor numbers,", "nasty tone,", "looking like a fool,", "bad hombre,"]
    part3 = ["got destroyed by my ratings.", "rigged the election.", "had a much smaller crowd.", "will pay for the wall."]
    part4 = ["So sad", "Apologize", "So true", "Media won't report", "Big trouble", "Fantastic job", "Stay tuned"]

Then I created a list of lists 
    best_words = [part1, part2, part3, part4]
    print(best_words)

Finaly I created the Generator
    sentence = []

    for part in best_words:
        r = random.randint(0, len(part) - 1)
        sentence.append(part[r])

    print(" ".join(sentence) + "!")
