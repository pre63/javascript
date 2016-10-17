const run = (generator) => {
  const iterate = (iteration) => {
    if (iteration.done) {
      return iteration.value;
    }
    const promise = iteration.value;
    return promise.then(value => iterate(iterator.next(value)));
  };
  const iterator = generator();
  iterate(iterator.next());
};
