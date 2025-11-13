class Caesar:
    @staticmethod
    def caesar_cipher_encryption(to_encrypt: str, hist: int = 2):
        alphabet =["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z"]
        encrypted = ""
        for word in to_encrypt:
            text = word.isalpha()
            if text:
                index1 = alphabet.index(word)
                to_hist_index = (index1 + hist) % len(alphabet)
                encrypted += alphabet[to_hist_index]
            else:
                encrypted += word
        return encrypted

    @staticmethod
    def caesar_cipher_decryption(encrypted: str, hist: int = 2):
        decrypted = ""
        alphabet = ["a","b","c","d","e","f","g","h","i","j","k","l","m","n","o","p","q","r","s","t","u","v","w","x","y","z"]
        for word in encrypted:
            text = word.isalpha()
            if text:
                index1 = alphabet.index(word)
                to_hist_index = index1 - hist
                decrypted += alphabet[to_hist_index]
            else:
                decrypted += word
        return decrypted


class RailFence:
    @classmethod
    def delete_spaces(cls, sentence: str):
        no_spaces = ""
        for letter in sentence:
            not_space = letter.isalpha()
            if not_space:
                no_spaces += letter
        return no_spaces

    @staticmethod
    def fence_encryption(to_encrypt: str):
        without_spaces = RailFence.delete_spaces(to_encrypt)
        rail1 = ""
        rail2 = ""
        for i in range(len(without_spaces)):
            if i % 2 == 0:
                rail1 += without_spaces[i]
            else:
                rail2 += without_spaces[i]
        return rail1 + rail2

    @staticmethod
    def fence_decryption(encrypted: str):
        rail1 = encrypted[:(len(encrypted // 2)) + 1]
        rail2 = encrypted[(len(encrypted // 2)) + 1:]
        decrypted_word = ""
        for i in range(len(rail1)):
            decrypted_word += rail1[i]
            decrypted_word += rail2[i]
        return decrypted_word
        # זה הקודים שיצרתי של הצפנה ופענוח של צופן גדר וצןפן קיסר והבאתי אןתם למיין בקריאה לדף הזה
