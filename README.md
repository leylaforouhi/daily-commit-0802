def is_palindrome(text):
    cleaned = text.replace(" ", "").lower()
    return cleaned == cleaned[::-1]

if __name__ == "__main__":
    samples = ["level", "Daily Commit", "radar"]
    for word in samples:
        print(f"{word}: {is_palindrome(word)}")
