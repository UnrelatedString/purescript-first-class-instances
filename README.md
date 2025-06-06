[![CI](https://github.com/UnrelatedString/purescript-first-class-instances/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/UnrelatedString/purescript-first-class-instances/actions/workflows/ci.yml)
![Latest Version Tag](https://img.shields.io/github/v/tag/UnrelatedString/purescript-first-class-instances)
[![Pursuit](https://pursuit.purescript.org/packages/purescript-first-class-instances/badge?)](https://pursuit.purescript.org/packages/purescript-first-class-instances)

# purescript-first-class-instances

Experimental / proof of concept package for representing typeclass instances as types themselves. Goals:

- [x] Provide a uniform mechanism for passing *representatives* of instances for whatever purposes may find that useful. such as the one I forgot until now was the whole reason I got back to this idea. Subsumed by [`instance-reflection`](https://github.com/UnrelatedString/purescript-instance-reflection) which provides this simpler and more stable feature without the volatility of all the other nonsense I'm trying to pull off here
- [ ] Substitute / augment the newtype idiom with the ability to refine to multiple "non-intersecting" instances simultaneously
- [ ] Make non-default orphan instances as painless as possible--in essence, this is the exact same thing as the existing newtype idiom, but made somewhat more difficult in PureScript because the mechanism for *including a class into the first class instance system* has to itself be orphan-friendly by relying on a user-defined type without it completely pervading everything
- [ ] Represent superclass relations as instance members / fundeps on the instance level
- [ ] Remember what the other two or so things were that I was going to write down ;_;
- [ ] Reflection and reification for instances
