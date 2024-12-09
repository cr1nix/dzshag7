class IterableWithGenerator:
    def __init__(self, start, end):
        self.start = start
        self.end = end

    def __iter__(self):

        for value in range(self.start, self.end + 1):
            yield value


iterable = IterableWithGenerator(1, 5)


for value in iterable:
    print(value)
