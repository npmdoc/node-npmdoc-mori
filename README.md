# api documentation for  [mori (v0.3.2)](https://github.com/swannodette/mori)  [![npm package](https://img.shields.io/npm/v/npmdoc-mori.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mori) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mori.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mori)
#### Persistent Data Structures for JavaScript

[![NPM](https://nodei.co/npm/mori.png?downloads=true)](https://www.npmjs.com/package/mori)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mori/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mori_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mori/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mori/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mori/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "David Nolen",
        "url": "https://github.com/swannodette"
    },
    "bugs": {
        "url": "https://github.com/swannodette/mori/issues"
    },
    "contributors": [
        {
            "name": "David Nolen",
            "url": "https://github.com/swannodette"
        }
    ],
    "dependencies": {},
    "description": "Persistent Data Structures for JavaScript",
    "devDependencies": {
        "immutable": "3.5.0",
        "jasmine-node": "1.7.0"
    },
    "directories": {
        "test": "./spec"
    },
    "dist": {
        "shasum": "1a53da165287f3bef0cab62398c4931bece80a3f",
        "tarball": "https://registry.npmjs.org/mori/-/mori-0.3.2.tgz"
    },
    "engines": {
        "node": ">=0.8.22"
    },
    "gitHead": "391df0b7cadf12236c982588d8336b44cefd0fa2",
    "homepage": "https://github.com/swannodette/mori",
    "keywords": [
        "data",
        "structure",
        "persistent",
        "clojure",
        "clojurescript",
        "map",
        "filter",
        "reduce"
    ],
    "licenses": [
        {
            "type": "EPL",
            "url": "https://raw.github.com/swannodette/mori/master/epl-v10.html"
        }
    ],
    "main": "./mori.js",
    "maintainers": [
        {
            "name": "dnolen",
            "email": "david.nolen@gmail.com"
        }
    ],
    "name": "mori",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/swannodette/mori.git"
    },
    "scripts": {
        "build": "./scripts/build.sh",
        "build-clean": "./scripts/build_clean.sh",
        "clean": "./scripts/clean.sh",
        "docs": "./scripts/docs.sh",
        "prepublish": "npm run-script build-clean",
        "test": "jasmine-node spec"
    },
    "version": "0.3.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mori](#apidoc.module.mori)
1.  [function <span class="apidocSignatureSpan">mori.</span>alterMeta (a, d, e)](#apidoc.element.mori.alterMeta)
1.  [function <span class="apidocSignatureSpan">mori.</span>apply (e, h, l, m, p, q)](#apidoc.element.mori.apply)
1.  [function <span class="apidocSignatureSpan">mori.</span>assoc (b, e, f, g)](#apidoc.element.mori.assoc)
1.  [function <span class="apidocSignatureSpan">mori.</span>assocIn (b, c, d)](#apidoc.element.mori.assocIn)
1.  [function <span class="apidocSignatureSpan">mori.</span>comp (c, f, g, h)](#apidoc.element.mori.comp)
1.  [function <span class="apidocSignatureSpan">mori.</span>compare (a, b)](#apidoc.element.mori.compare)
1.  [function <span class="apidocSignatureSpan">mori.</span>completing (c, e)](#apidoc.element.mori.completing)
1.  [function <span class="apidocSignatureSpan">mori.</span>concat (d, g, h)](#apidoc.element.mori.concat)
1.  [function <span class="apidocSignatureSpan">mori.</span>configure (a, b)](#apidoc.element.mori.configure)
1.  [function <span class="apidocSignatureSpan">mori.</span>conj (b, e, f)](#apidoc.element.mori.conj)
1.  [function <span class="apidocSignatureSpan">mori.</span>cons (a, b)](#apidoc.element.mori.cons)
1.  [function <span class="apidocSignatureSpan">mori.</span>constantly (a)](#apidoc.element.mori.constantly)
1.  [function <span class="apidocSignatureSpan">mori.</span>count (a)](#apidoc.element.mori.count)
1.  [function <span class="apidocSignatureSpan">mori.</span>curry (a, d)](#apidoc.element.mori.curry)
1.  [function <span class="apidocSignatureSpan">mori.</span>dec (a)](#apidoc.element.mori.dec)
1.  [function <span class="apidocSignatureSpan">mori.</span>dedupe (c)](#apidoc.element.mori.dedupe)
1.  [function <span class="apidocSignatureSpan">mori.</span>difference (b, e, f)](#apidoc.element.mori.difference)
1.  [function <span class="apidocSignatureSpan">mori.</span>disj (b, e, f)](#apidoc.element.mori.disj)
1.  [function <span class="apidocSignatureSpan">mori.</span>dissoc (b, e, f)](#apidoc.element.mori.dissoc)
1.  [function <span class="apidocSignatureSpan">mori.</span>distinct (a)](#apidoc.element.mori.distinct)
1.  [function <span class="apidocSignatureSpan">mori.</span>drop (c, e)](#apidoc.element.mori.drop)
1.  [function <span class="apidocSignatureSpan">mori.</span>dropWhile (c, e)](#apidoc.element.mori.dropWhile)
1.  [function <span class="apidocSignatureSpan">mori.</span>each (a, b)](#apidoc.element.mori.each)
1.  [function <span class="apidocSignatureSpan">mori.</span>eduction (a, b)](#apidoc.element.mori.eduction)
1.  [function <span class="apidocSignatureSpan">mori.</span>empty (a)](#apidoc.element.mori.empty)
1.  [function <span class="apidocSignatureSpan">mori.</span>equals (b, e, f)](#apidoc.element.mori.equals)
1.  [function <span class="apidocSignatureSpan">mori.</span>every (a, b)](#apidoc.element.mori.every)
1.  [function <span class="apidocSignatureSpan">mori.</span>filter (c, e)](#apidoc.element.mori.filter)
1.  [function <span class="apidocSignatureSpan">mori.</span>find (a, b)](#apidoc.element.mori.find)
1.  [function <span class="apidocSignatureSpan">mori.</span>first (a)](#apidoc.element.mori.first)
1.  [function <span class="apidocSignatureSpan">mori.</span>flatten (a)](#apidoc.element.mori.flatten)
1.  [function <span class="apidocSignatureSpan">mori.</span>fnil (d, f, g, h)](#apidoc.element.mori.fnil)
1.  [function <span class="apidocSignatureSpan">mori.</span>get (c, e, f)](#apidoc.element.mori.get)
1.  [function <span class="apidocSignatureSpan">mori.</span>getIn (c, e, f)](#apidoc.element.mori.getIn)
1.  [function <span class="apidocSignatureSpan">mori.</span>groupBy (a, b)](#apidoc.element.mori.groupBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>gt (a, d, e)](#apidoc.element.mori.gt)
1.  [function <span class="apidocSignatureSpan">mori.</span>gte (a, d, e)](#apidoc.element.mori.gte)
1.  [function <span class="apidocSignatureSpan">mori.</span>hasKey (a, b)](#apidoc.element.mori.hasKey)
1.  [function <span class="apidocSignatureSpan">mori.</span>hash (a)](#apidoc.element.mori.hash)
1.  [function <span class="apidocSignatureSpan">mori.</span>hashMap (a)](#apidoc.element.mori.hashMap)
1.  [function <span class="apidocSignatureSpan">mori.</span>identity (a)](#apidoc.element.mori.identity)
1.  [function <span class="apidocSignatureSpan">mori.</span>inc (a)](#apidoc.element.mori.inc)
1.  [function <span class="apidocSignatureSpan">mori.</span>index (a, b)](#apidoc.element.mori.index)
1.  [function <span class="apidocSignatureSpan">mori.</span>interleave (b, e, f)](#apidoc.element.mori.interleave)
1.  [function <span class="apidocSignatureSpan">mori.</span>interpose (a, b)](#apidoc.element.mori.interpose)
1.  [function <span class="apidocSignatureSpan">mori.</span>intersection (b, e, f)](#apidoc.element.mori.intersection)
1.  [function <span class="apidocSignatureSpan">mori.</span>into (c, e, f)](#apidoc.element.mori.into)
1.  [function <span class="apidocSignatureSpan">mori.</span>intoArray (d, c)](#apidoc.element.mori.intoArray)
1.  [function <span class="apidocSignatureSpan">mori.</span>isAssociative (a)](#apidoc.element.mori.isAssociative)
1.  [function <span class="apidocSignatureSpan">mori.</span>isCollection (a)](#apidoc.element.mori.isCollection)
1.  [function <span class="apidocSignatureSpan">mori.</span>isCounted (a)](#apidoc.element.mori.isCounted)
1.  [function <span class="apidocSignatureSpan">mori.</span>isEmpty (a)](#apidoc.element.mori.isEmpty)
1.  [function <span class="apidocSignatureSpan">mori.</span>isEven (a)](#apidoc.element.mori.isEven)
1.  [function <span class="apidocSignatureSpan">mori.</span>isIndexed (a)](#apidoc.element.mori.isIndexed)
1.  [function <span class="apidocSignatureSpan">mori.</span>isKeyword (a)](#apidoc.element.mori.isKeyword)
1.  [function <span class="apidocSignatureSpan">mori.</span>isList (a)](#apidoc.element.mori.isList)
1.  [function <span class="apidocSignatureSpan">mori.</span>isMap (a)](#apidoc.element.mori.isMap)
1.  [function <span class="apidocSignatureSpan">mori.</span>isOdd (a)](#apidoc.element.mori.isOdd)
1.  [function <span class="apidocSignatureSpan">mori.</span>isReduceable (a)](#apidoc.element.mori.isReduceable)
1.  [function <span class="apidocSignatureSpan">mori.</span>isReversible (a)](#apidoc.element.mori.isReversible)
1.  [function <span class="apidocSignatureSpan">mori.</span>isSeq (a)](#apidoc.element.mori.isSeq)
1.  [function <span class="apidocSignatureSpan">mori.</span>isSeqable (a)](#apidoc.element.mori.isSeqable)
1.  [function <span class="apidocSignatureSpan">mori.</span>isSequential (a)](#apidoc.element.mori.isSequential)
1.  [function <span class="apidocSignatureSpan">mori.</span>isSet (a)](#apidoc.element.mori.isSet)
1.  [function <span class="apidocSignatureSpan">mori.</span>isSubset (a, b)](#apidoc.element.mori.isSubset)
1.  [function <span class="apidocSignatureSpan">mori.</span>isSuperset (a, b)](#apidoc.element.mori.isSuperset)
1.  [function <span class="apidocSignatureSpan">mori.</span>isSymbol (a)](#apidoc.element.mori.isSymbol)
1.  [function <span class="apidocSignatureSpan">mori.</span>isVector (a)](#apidoc.element.mori.isVector)
1.  [function <span class="apidocSignatureSpan">mori.</span>iterate (b, c)](#apidoc.element.mori.iterate)
1.  [function <span class="apidocSignatureSpan">mori.</span>join (c, e, f)](#apidoc.element.mori.join)
1.  [function <span class="apidocSignatureSpan">mori.</span>juxt (a)](#apidoc.element.mori.juxt)
1.  [function <span class="apidocSignatureSpan">mori.</span>keep (c, e)](#apidoc.element.mori.keep)
1.  [function <span class="apidocSignatureSpan">mori.</span>keepIndexed (c, e)](#apidoc.element.mori.keepIndexed)
1.  [function <span class="apidocSignatureSpan">mori.</span>keys (a)](#apidoc.element.mori.keys)
1.  [function <span class="apidocSignatureSpan">mori.</span>keyword (c, e)](#apidoc.element.mori.keyword)
1.  [function <span class="apidocSignatureSpan">mori.</span>knit (a)](#apidoc.element.mori.knit)
1.  [function <span class="apidocSignatureSpan">mori.</span>last (a)](#apidoc.element.mori.last)
1.  [function <span class="apidocSignatureSpan">mori.</span>lazySeq (a)](#apidoc.element.mori.lazySeq)
1.  [function <span class="apidocSignatureSpan">mori.</span>list (a)](#apidoc.element.mori.list)
1.  [function <span class="apidocSignatureSpan">mori.</span>lt (a, d, e)](#apidoc.element.mori.lt)
1.  [function <span class="apidocSignatureSpan">mori.</span>lte (a, d, e)](#apidoc.element.mori.lte)
1.  [function <span class="apidocSignatureSpan">mori.</span>map (e, h, l, m, p)](#apidoc.element.mori.map)
1.  [function <span class="apidocSignatureSpan">mori.</span>mapIndexed (a, b)](#apidoc.element.mori.mapIndexed)
1.  [function <span class="apidocSignatureSpan">mori.</span>mapInvert (a)](#apidoc.element.mori.mapInvert)
1.  [function <span class="apidocSignatureSpan">mori.</span>mapcat (b, e)](#apidoc.element.mori.mapcat)
1.  [function <span class="apidocSignatureSpan">mori.</span>merge (a)](#apidoc.element.mori.merge)
1.  [function <span class="apidocSignatureSpan">mori.</span>mergeWith (a, d)](#apidoc.element.mori.mergeWith)
1.  [function <span class="apidocSignatureSpan">mori.</span>meta (a)](#apidoc.element.mori.meta)
1.  [function <span class="apidocSignatureSpan">mori.</span>mutable.assoc (a, d, e, f)](#apidoc.element.mori.mutable.assoc)
1.  [function <span class="apidocSignatureSpan">mori.</span>mutable.conj (b, e, f)](#apidoc.element.mori.mutable.conj)
1.  [function <span class="apidocSignatureSpan">mori.</span>mutable.disj (a, d, e)](#apidoc.element.mori.mutable.disj)
1.  [function <span class="apidocSignatureSpan">mori.</span>mutable.dissoc (a, d, e)](#apidoc.element.mori.mutable.dissoc)
1.  [function <span class="apidocSignatureSpan">mori.</span>next (a)](#apidoc.element.mori.next)
1.  [function <span class="apidocSignatureSpan">mori.</span>notEquals (b, e, f)](#apidoc.element.mori.notEquals)
1.  [function <span class="apidocSignatureSpan">mori.</span>nth (c, e, f)](#apidoc.element.mori.nth)
1.  [function <span class="apidocSignatureSpan">mori.</span>partial (d, g, h, l, m)](#apidoc.element.mori.partial)
1.  [function <span class="apidocSignatureSpan">mori.</span>partition (d, f, g, h)](#apidoc.element.mori.partition)
1.  [function <span class="apidocSignatureSpan">mori.</span>partitionAll (d, f, g)](#apidoc.element.mori.partitionAll)
1.  [function <span class="apidocSignatureSpan">mori.</span>partitionBy (c, e)](#apidoc.element.mori.partitionBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>peek (a)](#apidoc.element.mori.peek)
1.  [function <span class="apidocSignatureSpan">mori.</span>pipeline (a)](#apidoc.element.mori.pipeline)
1.  [function <span class="apidocSignatureSpan">mori.</span>pop (a)](#apidoc.element.mori.pop)
1.  [function <span class="apidocSignatureSpan">mori.</span>primSeq (c, e)](#apidoc.element.mori.primSeq)
1.  [function <span class="apidocSignatureSpan">mori.</span>project (a, b)](#apidoc.element.mori.project)
1.  [function <span class="apidocSignatureSpan">mori.</span>queue (a)](#apidoc.element.mori.queue)
1.  [function <span class="apidocSignatureSpan">mori.</span>range (e, g, h)](#apidoc.element.mori.range)
1.  [function <span class="apidocSignatureSpan">mori.</span>reduce (c, e, f)](#apidoc.element.mori.reduce)
1.  [function <span class="apidocSignatureSpan">mori.</span>reduceKV (a, b, c)](#apidoc.element.mori.reduceKV)
1.  [function <span class="apidocSignatureSpan">mori.</span>remove (c, e)](#apidoc.element.mori.remove)
1.  [function <span class="apidocSignatureSpan">mori.</span>rename (a, b)](#apidoc.element.mori.rename)
1.  [function <span class="apidocSignatureSpan">mori.</span>renameKeys (a, b)](#apidoc.element.mori.renameKeys)
1.  [function <span class="apidocSignatureSpan">mori.</span>repeat (c, e)](#apidoc.element.mori.repeat)
1.  [function <span class="apidocSignatureSpan">mori.</span>repeatedly (c, e)](#apidoc.element.mori.repeatedly)
1.  [function <span class="apidocSignatureSpan">mori.</span>resetMeta (a, b)](#apidoc.element.mori.resetMeta)
1.  [function <span class="apidocSignatureSpan">mori.</span>rest (a)](#apidoc.element.mori.rest)
1.  [function <span class="apidocSignatureSpan">mori.</span>reverse (a)](#apidoc.element.mori.reverse)
1.  [function <span class="apidocSignatureSpan">mori.</span>second (a)](#apidoc.element.mori.second)
1.  [function <span class="apidocSignatureSpan">mori.</span>selectKeys (a, b)](#apidoc.element.mori.selectKeys)
1.  [function <span class="apidocSignatureSpan">mori.</span>seq (a)](#apidoc.element.mori.seq)
1.  [function <span class="apidocSignatureSpan">mori.</span>sequence (b, e, f)](#apidoc.element.mori.sequence)
1.  [function <span class="apidocSignatureSpan">mori.</span>set (a)](#apidoc.element.mori.set)
1.  [function <span class="apidocSignatureSpan">mori.</span>some (a, b)](#apidoc.element.mori.some)
1.  [function <span class="apidocSignatureSpan">mori.</span>sort (c, e)](#apidoc.element.mori.sort)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortBy (c, e, f)](#apidoc.element.mori.sortBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortedMap (a)](#apidoc.element.mori.sortedMap)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortedMapBy (a, d)](#apidoc.element.mori.sortedMapBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortedSet (a)](#apidoc.element.mori.sortedSet)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortedSetBy (a, d)](#apidoc.element.mori.sortedSetBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>subseq (c, e, f, g, h)](#apidoc.element.mori.subseq)
1.  [function <span class="apidocSignatureSpan">mori.</span>subvec (c, e, f)](#apidoc.element.mori.subvec)
1.  [function <span class="apidocSignatureSpan">mori.</span>sum (a, d, e)](#apidoc.element.mori.sum)
1.  [function <span class="apidocSignatureSpan">mori.</span>symbol (c, e)](#apidoc.element.mori.symbol)
1.  [function <span class="apidocSignatureSpan">mori.</span>take (c, e)](#apidoc.element.mori.take)
1.  [function <span class="apidocSignatureSpan">mori.</span>takeNth (c, e)](#apidoc.element.mori.takeNth)
1.  [function <span class="apidocSignatureSpan">mori.</span>takeWhile (c, e)](#apidoc.element.mori.takeWhile)
1.  [function <span class="apidocSignatureSpan">mori.</span>toClj (c, e)](#apidoc.element.mori.toClj)
1.  [function <span class="apidocSignatureSpan">mori.</span>toJs (b)](#apidoc.element.mori.toJs)
1.  [function <span class="apidocSignatureSpan">mori.</span>transduce (c, e, f, g)](#apidoc.element.mori.transduce)
1.  [function <span class="apidocSignatureSpan">mori.</span>union (b, e, f)](#apidoc.element.mori.union)
1.  [function <span class="apidocSignatureSpan">mori.</span>updateIn (e, h, l, m, p, q, s)](#apidoc.element.mori.updateIn)
1.  [function <span class="apidocSignatureSpan">mori.</span>vals (a)](#apidoc.element.mori.vals)
1.  [function <span class="apidocSignatureSpan">mori.</span>varyMeta (f, l, m, p, q, s, u)](#apidoc.element.mori.varyMeta)
1.  [function <span class="apidocSignatureSpan">mori.</span>vector (a)](#apidoc.element.mori.vector)
1.  [function <span class="apidocSignatureSpan">mori.</span>withMeta (a, b)](#apidoc.element.mori.withMeta)
1.  [function <span class="apidocSignatureSpan">mori.</span>zipmap (a, b)](#apidoc.element.mori.zipmap)
1.  object <span class="apidocSignatureSpan">mori.</span>mutable

#### [module mori.alterMeta](#apidoc.module.mori.alterMeta)
1.  [function <span class="apidocSignatureSpan">mori.</span>alterMeta (a, d, e)](#apidoc.element.mori.alterMeta.alterMeta)
1.  [function <span class="apidocSignatureSpan">mori.alterMeta.</span>d (a, b, e)](#apidoc.element.mori.alterMeta.d)
1.  [function <span class="apidocSignatureSpan">mori.alterMeta.</span>f (a)](#apidoc.element.mori.alterMeta.f)
1.  number <span class="apidocSignatureSpan">mori.alterMeta.</span>i

#### [module mori.apply](#apidoc.module.mori.apply)
1.  [function <span class="apidocSignatureSpan">mori.</span>apply ()](#apidoc.element.mori.apply.apply)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>a (a, b)](#apidoc.element.mori.apply.a)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>c (a, b, c)](#apidoc.element.mori.apply.c)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>d (a, c, d, e, f, g)](#apidoc.element.mori.apply.d)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>f (a)](#apidoc.element.mori.apply.f)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>f2 (a, b)](#apidoc.element.mori.apply.f2)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>f3 (a, b, c)](#apidoc.element.mori.apply.f3)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>f4 (a, b, c, d)](#apidoc.element.mori.apply.f4)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>f5 (a, b, c, d, e)](#apidoc.element.mori.apply.f5)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>n (a, b, c, d)](#apidoc.element.mori.apply.n)
1.  [function <span class="apidocSignatureSpan">mori.apply.</span>r (a, b, c, d, e)](#apidoc.element.mori.apply.r)
1.  number <span class="apidocSignatureSpan">mori.apply.</span>i
1.  object <span class="apidocSignatureSpan">mori.apply.</span>fn

#### [module mori.assoc](#apidoc.module.mori.assoc)
1.  [function <span class="apidocSignatureSpan">mori.</span>assoc (b, e, f, g)](#apidoc.element.mori.assoc.assoc)
1.  [function <span class="apidocSignatureSpan">mori.assoc.</span>c (a, b, c)](#apidoc.element.mori.assoc.c)
1.  [function <span class="apidocSignatureSpan">mori.assoc.</span>d (a, d, e, l)](#apidoc.element.mori.assoc.d)
1.  [function <span class="apidocSignatureSpan">mori.assoc.</span>f (a)](#apidoc.element.mori.assoc.f)
1.  [function <span class="apidocSignatureSpan">mori.assoc.</span>f3 (a, b, c)](#apidoc.element.mori.assoc.f3)
1.  number <span class="apidocSignatureSpan">mori.assoc.</span>i
1.  object <span class="apidocSignatureSpan">mori.assoc.</span>fn

#### [module mori.comp](#apidoc.module.mori.comp)
1.  [function <span class="apidocSignatureSpan">mori.</span>comp (c, f, g, h)](#apidoc.element.mori.comp.comp)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>a (a, b)](#apidoc.element.mori.comp.a)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>b (a)](#apidoc.element.mori.comp.b)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>c (a, b, c)](#apidoc.element.mori.comp.c)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>d (a, c, d, e)](#apidoc.element.mori.comp.d)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>f (a)](#apidoc.element.mori.comp.f)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>f0 ()](#apidoc.element.mori.comp.f0)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>f1 (a)](#apidoc.element.mori.comp.f1)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>f2 (a, b)](#apidoc.element.mori.comp.f2)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>f3 (a, b, c)](#apidoc.element.mori.comp.f3)
1.  [function <span class="apidocSignatureSpan">mori.comp.</span>l ()](#apidoc.element.mori.comp.l)
1.  number <span class="apidocSignatureSpan">mori.comp.</span>i
1.  object <span class="apidocSignatureSpan">mori.comp.</span>fn

#### [module mori.completing](#apidoc.module.mori.completing)
1.  [function <span class="apidocSignatureSpan">mori.</span>completing (c, e)](#apidoc.element.mori.completing.completing)
1.  [function <span class="apidocSignatureSpan">mori.completing.</span>a (a, b)](#apidoc.element.mori.completing.a)
1.  [function <span class="apidocSignatureSpan">mori.completing.</span>b (a)](#apidoc.element.mori.completing.b)
1.  [function <span class="apidocSignatureSpan">mori.completing.</span>f1 (a)](#apidoc.element.mori.completing.f1)
1.  [function <span class="apidocSignatureSpan">mori.completing.</span>f2 (a, b)](#apidoc.element.mori.completing.f2)

#### [module mori.concat](#apidoc.module.mori.concat)
1.  [function <span class="apidocSignatureSpan">mori.</span>concat (d, g, h)](#apidoc.element.mori.concat.concat)
1.  [function <span class="apidocSignatureSpan">mori.concat.</span>a (a, b)](#apidoc.element.mori.concat.a)
1.  [function <span class="apidocSignatureSpan">mori.concat.</span>b (a)](#apidoc.element.mori.concat.b)
1.  [function <span class="apidocSignatureSpan">mori.concat.</span>d (a, c, e)](#apidoc.element.mori.concat.d)
1.  [function <span class="apidocSignatureSpan">mori.concat.</span>f (a)](#apidoc.element.mori.concat.f)
1.  [function <span class="apidocSignatureSpan">mori.concat.</span>f0 ()](#apidoc.element.mori.concat.f0)
1.  [function <span class="apidocSignatureSpan">mori.concat.</span>f1 (a)](#apidoc.element.mori.concat.f1)
1.  [function <span class="apidocSignatureSpan">mori.concat.</span>f2 (a, b)](#apidoc.element.mori.concat.f2)
1.  [function <span class="apidocSignatureSpan">mori.concat.</span>l ()](#apidoc.element.mori.concat.l)
1.  number <span class="apidocSignatureSpan">mori.concat.</span>i
1.  object <span class="apidocSignatureSpan">mori.concat.</span>fn

#### [module mori.conj](#apidoc.module.mori.conj)
1.  [function <span class="apidocSignatureSpan">mori.</span>conj (b, e, f)](#apidoc.element.mori.conj.conj)
1.  [function <span class="apidocSignatureSpan">mori.conj.</span>a (a, b)](#apidoc.element.mori.conj.a)
1.  [function <span class="apidocSignatureSpan">mori.conj.</span>b (a)](#apidoc.element.mori.conj.b)
1.  [function <span class="apidocSignatureSpan">mori.conj.</span>d (a, d, e)](#apidoc.element.mori.conj.d)
1.  [function <span class="apidocSignatureSpan">mori.conj.</span>f (a)](#apidoc.element.mori.conj.f)
1.  [function <span class="apidocSignatureSpan">mori.conj.</span>f0 ()](#apidoc.element.mori.conj.f0)
1.  [function <span class="apidocSignatureSpan">mori.conj.</span>f1 (a)](#apidoc.element.mori.conj.f1)
1.  [function <span class="apidocSignatureSpan">mori.conj.</span>f2 (a, b)](#apidoc.element.mori.conj.f2)
1.  [function <span class="apidocSignatureSpan">mori.conj.</span>l ()](#apidoc.element.mori.conj.l)
1.  number <span class="apidocSignatureSpan">mori.conj.</span>i
1.  object <span class="apidocSignatureSpan">mori.conj.</span>fn

#### [module mori.curry](#apidoc.module.mori.curry)
1.  [function <span class="apidocSignatureSpan">mori.</span>curry (a, d)](#apidoc.element.mori.curry.curry)
1.  [function <span class="apidocSignatureSpan">mori.curry.</span>d (a, b)](#apidoc.element.mori.curry.d)
1.  [function <span class="apidocSignatureSpan">mori.curry.</span>f (a)](#apidoc.element.mori.curry.f)
1.  number <span class="apidocSignatureSpan">mori.curry.</span>i

#### [module mori.dedupe](#apidoc.module.mori.dedupe)
1.  [function <span class="apidocSignatureSpan">mori.</span>dedupe (c)](#apidoc.element.mori.dedupe.dedupe)
1.  [function <span class="apidocSignatureSpan">mori.dedupe.</span>b (a)](#apidoc.element.mori.dedupe.b)
1.  [function <span class="apidocSignatureSpan">mori.dedupe.</span>f0 ()](#apidoc.element.mori.dedupe.f0)
1.  [function <span class="apidocSignatureSpan">mori.dedupe.</span>f1 (a)](#apidoc.element.mori.dedupe.f1)
1.  [function <span class="apidocSignatureSpan">mori.dedupe.</span>l ()](#apidoc.element.mori.dedupe.l)

#### [module mori.difference](#apidoc.module.mori.difference)
1.  [function <span class="apidocSignatureSpan">mori.</span>difference (b, e, f)](#apidoc.element.mori.difference.difference)
1.  [function <span class="apidocSignatureSpan">mori.difference.</span>a (a, b)](#apidoc.element.mori.difference.a)
1.  [function <span class="apidocSignatureSpan">mori.difference.</span>b (a)](#apidoc.element.mori.difference.b)
1.  [function <span class="apidocSignatureSpan">mori.difference.</span>d (a, d, e)](#apidoc.element.mori.difference.d)
1.  [function <span class="apidocSignatureSpan">mori.difference.</span>f (a)](#apidoc.element.mori.difference.f)
1.  [function <span class="apidocSignatureSpan">mori.difference.</span>f1 (a)](#apidoc.element.mori.difference.f1)
1.  [function <span class="apidocSignatureSpan">mori.difference.</span>f2 (a, b)](#apidoc.element.mori.difference.f2)
1.  number <span class="apidocSignatureSpan">mori.difference.</span>i
1.  object <span class="apidocSignatureSpan">mori.difference.</span>fn

#### [module mori.disj](#apidoc.module.mori.disj)
1.  [function <span class="apidocSignatureSpan">mori.</span>disj (b, e, f)](#apidoc.element.mori.disj.disj)
1.  [function <span class="apidocSignatureSpan">mori.disj.</span>a (a, b)](#apidoc.element.mori.disj.a)
1.  [function <span class="apidocSignatureSpan">mori.disj.</span>b (a)](#apidoc.element.mori.disj.b)
1.  [function <span class="apidocSignatureSpan">mori.disj.</span>d (a, d, e)](#apidoc.element.mori.disj.d)
1.  [function <span class="apidocSignatureSpan">mori.disj.</span>f (a)](#apidoc.element.mori.disj.f)
1.  [function <span class="apidocSignatureSpan">mori.disj.</span>f1 (a)](#apidoc.element.mori.disj.f1)
1.  [function <span class="apidocSignatureSpan">mori.disj.</span>f2 (a, b)](#apidoc.element.mori.disj.f2)
1.  number <span class="apidocSignatureSpan">mori.disj.</span>i
1.  object <span class="apidocSignatureSpan">mori.disj.</span>fn

#### [module mori.dissoc](#apidoc.module.mori.dissoc)
1.  [function <span class="apidocSignatureSpan">mori.</span>dissoc (b, e, f)](#apidoc.element.mori.dissoc.dissoc)
1.  [function <span class="apidocSignatureSpan">mori.dissoc.</span>a (a, b)](#apidoc.element.mori.dissoc.a)
1.  [function <span class="apidocSignatureSpan">mori.dissoc.</span>b (a)](#apidoc.element.mori.dissoc.b)
1.  [function <span class="apidocSignatureSpan">mori.dissoc.</span>d (a, d, e)](#apidoc.element.mori.dissoc.d)
1.  [function <span class="apidocSignatureSpan">mori.dissoc.</span>f (a)](#apidoc.element.mori.dissoc.f)
1.  [function <span class="apidocSignatureSpan">mori.dissoc.</span>f1 (a)](#apidoc.element.mori.dissoc.f1)
1.  [function <span class="apidocSignatureSpan">mori.dissoc.</span>f2 (a, b)](#apidoc.element.mori.dissoc.f2)
1.  number <span class="apidocSignatureSpan">mori.dissoc.</span>i
1.  object <span class="apidocSignatureSpan">mori.dissoc.</span>fn

#### [module mori.drop](#apidoc.module.mori.drop)
1.  [function <span class="apidocSignatureSpan">mori.</span>drop (c, e)](#apidoc.element.mori.drop.drop)
1.  [function <span class="apidocSignatureSpan">mori.drop.</span>a (a, b)](#apidoc.element.mori.drop.a)
1.  [function <span class="apidocSignatureSpan">mori.drop.</span>b (a)](#apidoc.element.mori.drop.b)
1.  [function <span class="apidocSignatureSpan">mori.drop.</span>f1 (a)](#apidoc.element.mori.drop.f1)
1.  [function <span class="apidocSignatureSpan">mori.drop.</span>f2 (a, b)](#apidoc.element.mori.drop.f2)

#### [module mori.dropWhile](#apidoc.module.mori.dropWhile)
1.  [function <span class="apidocSignatureSpan">mori.</span>dropWhile (c, e)](#apidoc.element.mori.dropWhile.dropWhile)
1.  [function <span class="apidocSignatureSpan">mori.dropWhile.</span>a (a, b)](#apidoc.element.mori.dropWhile.a)
1.  [function <span class="apidocSignatureSpan">mori.dropWhile.</span>b (a)](#apidoc.element.mori.dropWhile.b)
1.  [function <span class="apidocSignatureSpan">mori.dropWhile.</span>f1 (a)](#apidoc.element.mori.dropWhile.f1)
1.  [function <span class="apidocSignatureSpan">mori.dropWhile.</span>f2 (a, b)](#apidoc.element.mori.dropWhile.f2)

#### [module mori.equals](#apidoc.module.mori.equals)
1.  [function <span class="apidocSignatureSpan">mori.</span>equals (b, e, f)](#apidoc.element.mori.equals.equals)
1.  [function <span class="apidocSignatureSpan">mori.equals.</span>a (a, b)](#apidoc.element.mori.equals.a)
1.  [function <span class="apidocSignatureSpan">mori.equals.</span>b ()](#apidoc.element.mori.equals.b)
1.  [function <span class="apidocSignatureSpan">mori.equals.</span>d (a, d, e)](#apidoc.element.mori.equals.d)
1.  [function <span class="apidocSignatureSpan">mori.equals.</span>f (a)](#apidoc.element.mori.equals.f)
1.  [function <span class="apidocSignatureSpan">mori.equals.</span>f1 ()](#apidoc.element.mori.equals.f1)
1.  [function <span class="apidocSignatureSpan">mori.equals.</span>f2 (a, b)](#apidoc.element.mori.equals.f2)
1.  number <span class="apidocSignatureSpan">mori.equals.</span>i
1.  object <span class="apidocSignatureSpan">mori.equals.</span>fn

#### [module mori.filter](#apidoc.module.mori.filter)
1.  [function <span class="apidocSignatureSpan">mori.</span>filter (c, e)](#apidoc.element.mori.filter.filter)
1.  [function <span class="apidocSignatureSpan">mori.filter.</span>a (a, b)](#apidoc.element.mori.filter.a)
1.  [function <span class="apidocSignatureSpan">mori.filter.</span>b (a)](#apidoc.element.mori.filter.b)
1.  [function <span class="apidocSignatureSpan">mori.filter.</span>f1 (a)](#apidoc.element.mori.filter.f1)
1.  [function <span class="apidocSignatureSpan">mori.filter.</span>f2 (a, b)](#apidoc.element.mori.filter.f2)

#### [module mori.fnil](#apidoc.module.mori.fnil)
1.  [function <span class="apidocSignatureSpan">mori.</span>fnil (d, f, g, h)](#apidoc.element.mori.fnil.fnil)
1.  [function <span class="apidocSignatureSpan">mori.fnil.</span>a (a, b)](#apidoc.element.mori.fnil.a)
1.  [function <span class="apidocSignatureSpan">mori.fnil.</span>c (a, b, c)](#apidoc.element.mori.fnil.c)
1.  [function <span class="apidocSignatureSpan">mori.fnil.</span>f2 (a, b)](#apidoc.element.mori.fnil.f2)
1.  [function <span class="apidocSignatureSpan">mori.fnil.</span>f3 (a, b, c)](#apidoc.element.mori.fnil.f3)
1.  [function <span class="apidocSignatureSpan">mori.fnil.</span>f4 (a, b, c, d)](#apidoc.element.mori.fnil.f4)
1.  [function <span class="apidocSignatureSpan">mori.fnil.</span>n (a, b, c, d)](#apidoc.element.mori.fnil.n)

#### [module mori.get](#apidoc.module.mori.get)
1.  [function <span class="apidocSignatureSpan">mori.</span>get (c, e, f)](#apidoc.element.mori.get.get)
1.  [function <span class="apidocSignatureSpan">mori.get.</span>a (a, b)](#apidoc.element.mori.get.a)
1.  [function <span class="apidocSignatureSpan">mori.get.</span>c (a, b, c)](#apidoc.element.mori.get.c)
1.  [function <span class="apidocSignatureSpan">mori.get.</span>f2 (a, b)](#apidoc.element.mori.get.f2)
1.  [function <span class="apidocSignatureSpan">mori.get.</span>f3 (a, b, c)](#apidoc.element.mori.get.f3)

#### [module mori.getIn](#apidoc.module.mori.getIn)
1.  [function <span class="apidocSignatureSpan">mori.</span>getIn (c, e, f)](#apidoc.element.mori.getIn.getIn)
1.  [function <span class="apidocSignatureSpan">mori.getIn.</span>a (a, b)](#apidoc.element.mori.getIn.a)
1.  [function <span class="apidocSignatureSpan">mori.getIn.</span>c (a, b, c)](#apidoc.element.mori.getIn.c)
1.  [function <span class="apidocSignatureSpan">mori.getIn.</span>f2 (a, b)](#apidoc.element.mori.getIn.f2)
1.  [function <span class="apidocSignatureSpan">mori.getIn.</span>f3 (a, b, c)](#apidoc.element.mori.getIn.f3)

#### [module mori.gt](#apidoc.module.mori.gt)
1.  [function <span class="apidocSignatureSpan">mori.</span>gt (a, d, e)](#apidoc.element.mori.gt.gt)
1.  [function <span class="apidocSignatureSpan">mori.gt.</span>a (a, b)](#apidoc.element.mori.gt.a)
1.  [function <span class="apidocSignatureSpan">mori.gt.</span>b ()](#apidoc.element.mori.gt.b)
1.  [function <span class="apidocSignatureSpan">mori.gt.</span>d (a, c, d)](#apidoc.element.mori.gt.d)
1.  [function <span class="apidocSignatureSpan">mori.gt.</span>f (a)](#apidoc.element.mori.gt.f)
1.  [function <span class="apidocSignatureSpan">mori.gt.</span>f1 ()](#apidoc.element.mori.gt.f1)
1.  [function <span class="apidocSignatureSpan">mori.gt.</span>f2 (a, b)](#apidoc.element.mori.gt.f2)
1.  number <span class="apidocSignatureSpan">mori.gt.</span>i
1.  object <span class="apidocSignatureSpan">mori.gt.</span>fn

#### [module mori.gte](#apidoc.module.mori.gte)
1.  [function <span class="apidocSignatureSpan">mori.</span>gte (a, d, e)](#apidoc.element.mori.gte.gte)
1.  [function <span class="apidocSignatureSpan">mori.gte.</span>a (a, b)](#apidoc.element.mori.gte.a)
1.  [function <span class="apidocSignatureSpan">mori.gte.</span>b ()](#apidoc.element.mori.gte.b)
1.  [function <span class="apidocSignatureSpan">mori.gte.</span>d (a, c, d)](#apidoc.element.mori.gte.d)
1.  [function <span class="apidocSignatureSpan">mori.gte.</span>f (a)](#apidoc.element.mori.gte.f)
1.  [function <span class="apidocSignatureSpan">mori.gte.</span>f1 ()](#apidoc.element.mori.gte.f1)
1.  [function <span class="apidocSignatureSpan">mori.gte.</span>f2 (a, b)](#apidoc.element.mori.gte.f2)
1.  number <span class="apidocSignatureSpan">mori.gte.</span>i
1.  object <span class="apidocSignatureSpan">mori.gte.</span>fn

#### [module mori.hashMap](#apidoc.module.mori.hashMap)
1.  [function <span class="apidocSignatureSpan">mori.</span>hashMap (a)](#apidoc.element.mori.hashMap.hashMap)
1.  [function <span class="apidocSignatureSpan">mori.hashMap.</span>d (a)](#apidoc.element.mori.hashMap.d)
1.  [function <span class="apidocSignatureSpan">mori.hashMap.</span>f (a)](#apidoc.element.mori.hashMap.f)
1.  number <span class="apidocSignatureSpan">mori.hashMap.</span>i

#### [module mori.interleave](#apidoc.module.mori.interleave)
1.  [function <span class="apidocSignatureSpan">mori.</span>interleave (b, e, f)](#apidoc.element.mori.interleave.interleave)
1.  [function <span class="apidocSignatureSpan">mori.interleave.</span>a (a, c)](#apidoc.element.mori.interleave.a)
1.  [function <span class="apidocSignatureSpan">mori.interleave.</span>d (a, d, e)](#apidoc.element.mori.interleave.d)
1.  [function <span class="apidocSignatureSpan">mori.interleave.</span>f (a)](#apidoc.element.mori.interleave.f)
1.  [function <span class="apidocSignatureSpan">mori.interleave.</span>f2 (a, c)](#apidoc.element.mori.interleave.f2)
1.  number <span class="apidocSignatureSpan">mori.interleave.</span>i
1.  object <span class="apidocSignatureSpan">mori.interleave.</span>fn

#### [module mori.intersection](#apidoc.module.mori.intersection)
1.  [function <span class="apidocSignatureSpan">mori.</span>intersection (b, e, f)](#apidoc.element.mori.intersection.intersection)
1.  [function <span class="apidocSignatureSpan">mori.intersection.</span>a (a, b)](#apidoc.element.mori.intersection.a)
1.  [function <span class="apidocSignatureSpan">mori.intersection.</span>b (a)](#apidoc.element.mori.intersection.b)
1.  [function <span class="apidocSignatureSpan">mori.intersection.</span>d (a, d, e)](#apidoc.element.mori.intersection.d)
1.  [function <span class="apidocSignatureSpan">mori.intersection.</span>f (a)](#apidoc.element.mori.intersection.f)
1.  [function <span class="apidocSignatureSpan">mori.intersection.</span>f1 (a)](#apidoc.element.mori.intersection.f1)
1.  [function <span class="apidocSignatureSpan">mori.intersection.</span>f2 (a, b)](#apidoc.element.mori.intersection.f2)
1.  number <span class="apidocSignatureSpan">mori.intersection.</span>i
1.  object <span class="apidocSignatureSpan">mori.intersection.</span>fn

#### [module mori.into](#apidoc.module.mori.into)
1.  [function <span class="apidocSignatureSpan">mori.</span>into (c, e, f)](#apidoc.element.mori.into.into)
1.  [function <span class="apidocSignatureSpan">mori.into.</span>a (a, b)](#apidoc.element.mori.into.a)
1.  [function <span class="apidocSignatureSpan">mori.into.</span>c (a, b, c)](#apidoc.element.mori.into.c)
1.  [function <span class="apidocSignatureSpan">mori.into.</span>f2 (a, b)](#apidoc.element.mori.into.f2)
1.  [function <span class="apidocSignatureSpan">mori.into.</span>f3 (a, b, c)](#apidoc.element.mori.into.f3)

#### [module mori.intoArray](#apidoc.module.mori.intoArray)
1.  [function <span class="apidocSignatureSpan">mori.</span>intoArray (d, c)](#apidoc.element.mori.intoArray.intoArray)
1.  [function <span class="apidocSignatureSpan">mori.intoArray.</span>a (a, b)](#apidoc.element.mori.intoArray.a)
1.  [function <span class="apidocSignatureSpan">mori.intoArray.</span>b (a)](#apidoc.element.mori.intoArray.b)
1.  [function <span class="apidocSignatureSpan">mori.intoArray.</span>f1 (a)](#apidoc.element.mori.intoArray.f1)
1.  [function <span class="apidocSignatureSpan">mori.intoArray.</span>f2 (a, b)](#apidoc.element.mori.intoArray.f2)

#### [module mori.join](#apidoc.module.mori.join)
1.  [function <span class="apidocSignatureSpan">mori.</span>join (c, e, f)](#apidoc.element.mori.join.join)
1.  [function <span class="apidocSignatureSpan">mori.join.</span>a (a, b)](#apidoc.element.mori.join.a)
1.  [function <span class="apidocSignatureSpan">mori.join.</span>c (a, b, c)](#apidoc.element.mori.join.c)
1.  [function <span class="apidocSignatureSpan">mori.join.</span>f2 (a, b)](#apidoc.element.mori.join.f2)
1.  [function <span class="apidocSignatureSpan">mori.join.</span>f3 (a, b, c)](#apidoc.element.mori.join.f3)

#### [module mori.juxt](#apidoc.module.mori.juxt)
1.  [function <span class="apidocSignatureSpan">mori.</span>juxt (a)](#apidoc.element.mori.juxt.juxt)
1.  [function <span class="apidocSignatureSpan">mori.juxt.</span>d (a)](#apidoc.element.mori.juxt.d)
1.  [function <span class="apidocSignatureSpan">mori.juxt.</span>f (a)](#apidoc.element.mori.juxt.f)
1.  number <span class="apidocSignatureSpan">mori.juxt.</span>i

#### [module mori.keep](#apidoc.module.mori.keep)
1.  [function <span class="apidocSignatureSpan">mori.</span>keep (c, e)](#apidoc.element.mori.keep.keep)
1.  [function <span class="apidocSignatureSpan">mori.keep.</span>a (a, b)](#apidoc.element.mori.keep.a)
1.  [function <span class="apidocSignatureSpan">mori.keep.</span>b (a)](#apidoc.element.mori.keep.b)
1.  [function <span class="apidocSignatureSpan">mori.keep.</span>f1 (a)](#apidoc.element.mori.keep.f1)
1.  [function <span class="apidocSignatureSpan">mori.keep.</span>f2 (a, b)](#apidoc.element.mori.keep.f2)

#### [module mori.keepIndexed](#apidoc.module.mori.keepIndexed)
1.  [function <span class="apidocSignatureSpan">mori.</span>keepIndexed (c, e)](#apidoc.element.mori.keepIndexed.keepIndexed)
1.  [function <span class="apidocSignatureSpan">mori.keepIndexed.</span>a (a, b)](#apidoc.element.mori.keepIndexed.a)
1.  [function <span class="apidocSignatureSpan">mori.keepIndexed.</span>b (a)](#apidoc.element.mori.keepIndexed.b)
1.  [function <span class="apidocSignatureSpan">mori.keepIndexed.</span>f1 (a)](#apidoc.element.mori.keepIndexed.f1)
1.  [function <span class="apidocSignatureSpan">mori.keepIndexed.</span>f2 (a, b)](#apidoc.element.mori.keepIndexed.f2)

#### [module mori.keyword](#apidoc.module.mori.keyword)
1.  [function <span class="apidocSignatureSpan">mori.</span>keyword (c, e)](#apidoc.element.mori.keyword.keyword)
1.  [function <span class="apidocSignatureSpan">mori.keyword.</span>a (a, b)](#apidoc.element.mori.keyword.a)
1.  [function <span class="apidocSignatureSpan">mori.keyword.</span>b (a)](#apidoc.element.mori.keyword.b)
1.  [function <span class="apidocSignatureSpan">mori.keyword.</span>f1 (a)](#apidoc.element.mori.keyword.f1)
1.  [function <span class="apidocSignatureSpan">mori.keyword.</span>f2 (a, b)](#apidoc.element.mori.keyword.f2)

#### [module mori.knit](#apidoc.module.mori.knit)
1.  [function <span class="apidocSignatureSpan">mori.</span>knit (a)](#apidoc.element.mori.knit.knit)
1.  [function <span class="apidocSignatureSpan">mori.knit.</span>d (a)](#apidoc.element.mori.knit.d)
1.  [function <span class="apidocSignatureSpan">mori.knit.</span>f (a)](#apidoc.element.mori.knit.f)
1.  number <span class="apidocSignatureSpan">mori.knit.</span>i

#### [module mori.list](#apidoc.module.mori.list)
1.  [function <span class="apidocSignatureSpan">mori.</span>list (a)](#apidoc.element.mori.list.list)
1.  [function <span class="apidocSignatureSpan">mori.list.</span>d (a)](#apidoc.element.mori.list.d)
1.  [function <span class="apidocSignatureSpan">mori.list.</span>f (a)](#apidoc.element.mori.list.f)
1.  number <span class="apidocSignatureSpan">mori.list.</span>i

#### [module mori.lt](#apidoc.module.mori.lt)
1.  [function <span class="apidocSignatureSpan">mori.</span>lt (a, d, e)](#apidoc.element.mori.lt.lt)
1.  [function <span class="apidocSignatureSpan">mori.lt.</span>a (a, b)](#apidoc.element.mori.lt.a)
1.  [function <span class="apidocSignatureSpan">mori.lt.</span>b ()](#apidoc.element.mori.lt.b)
1.  [function <span class="apidocSignatureSpan">mori.lt.</span>d (a, c, d)](#apidoc.element.mori.lt.d)
1.  [function <span class="apidocSignatureSpan">mori.lt.</span>f (a)](#apidoc.element.mori.lt.f)
1.  [function <span class="apidocSignatureSpan">mori.lt.</span>f1 ()](#apidoc.element.mori.lt.f1)
1.  [function <span class="apidocSignatureSpan">mori.lt.</span>f2 (a, b)](#apidoc.element.mori.lt.f2)
1.  number <span class="apidocSignatureSpan">mori.lt.</span>i
1.  object <span class="apidocSignatureSpan">mori.lt.</span>fn

#### [module mori.lte](#apidoc.module.mori.lte)
1.  [function <span class="apidocSignatureSpan">mori.</span>lte (a, d, e)](#apidoc.element.mori.lte.lte)
1.  [function <span class="apidocSignatureSpan">mori.lte.</span>a (a, b)](#apidoc.element.mori.lte.a)
1.  [function <span class="apidocSignatureSpan">mori.lte.</span>b ()](#apidoc.element.mori.lte.b)
1.  [function <span class="apidocSignatureSpan">mori.lte.</span>d (a, c, d)](#apidoc.element.mori.lte.d)
1.  [function <span class="apidocSignatureSpan">mori.lte.</span>f (a)](#apidoc.element.mori.lte.f)
1.  [function <span class="apidocSignatureSpan">mori.lte.</span>f1 ()](#apidoc.element.mori.lte.f1)
1.  [function <span class="apidocSignatureSpan">mori.lte.</span>f2 (a, b)](#apidoc.element.mori.lte.f2)
1.  number <span class="apidocSignatureSpan">mori.lte.</span>i
1.  object <span class="apidocSignatureSpan">mori.lte.</span>fn

#### [module mori.map](#apidoc.module.mori.map)
1.  [function <span class="apidocSignatureSpan">mori.</span>map (e, h, l, m, p)](#apidoc.element.mori.map.map)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>a (a, b)](#apidoc.element.mori.map.a)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>b (a)](#apidoc.element.mori.map.b)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>c (a, b, c)](#apidoc.element.mori.map.c)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>d (a, c, d, f, g)](#apidoc.element.mori.map.d)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>f (a)](#apidoc.element.mori.map.f)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>f1 (a)](#apidoc.element.mori.map.f1)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>f2 (a, b)](#apidoc.element.mori.map.f2)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>f3 (a, b, c)](#apidoc.element.mori.map.f3)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>f4 (a, b, c, d)](#apidoc.element.mori.map.f4)
1.  [function <span class="apidocSignatureSpan">mori.map.</span>n (a, b, c, d)](#apidoc.element.mori.map.n)
1.  number <span class="apidocSignatureSpan">mori.map.</span>i
1.  object <span class="apidocSignatureSpan">mori.map.</span>fn

#### [module mori.mapcat](#apidoc.module.mori.mapcat)
1.  [function <span class="apidocSignatureSpan">mori.</span>mapcat (b, e)](#apidoc.element.mori.mapcat.mapcat)
1.  [function <span class="apidocSignatureSpan">mori.mapcat.</span>b (a)](#apidoc.element.mori.mapcat.b)
1.  [function <span class="apidocSignatureSpan">mori.mapcat.</span>d (a, c)](#apidoc.element.mori.mapcat.d)
1.  [function <span class="apidocSignatureSpan">mori.mapcat.</span>f (a)](#apidoc.element.mori.mapcat.f)
1.  [function <span class="apidocSignatureSpan">mori.mapcat.</span>f1 (a)](#apidoc.element.mori.mapcat.f1)
1.  number <span class="apidocSignatureSpan">mori.mapcat.</span>i
1.  object <span class="apidocSignatureSpan">mori.mapcat.</span>fn

#### [module mori.merge](#apidoc.module.mori.merge)
1.  [function <span class="apidocSignatureSpan">mori.</span>merge (a)](#apidoc.element.mori.merge.merge)
1.  [function <span class="apidocSignatureSpan">mori.merge.</span>d (a)](#apidoc.element.mori.merge.d)
1.  [function <span class="apidocSignatureSpan">mori.merge.</span>f (a)](#apidoc.element.mori.merge.f)
1.  number <span class="apidocSignatureSpan">mori.merge.</span>i

#### [module mori.mergeWith](#apidoc.module.mori.mergeWith)
1.  [function <span class="apidocSignatureSpan">mori.</span>mergeWith (a, d)](#apidoc.element.mori.mergeWith.mergeWith)
1.  [function <span class="apidocSignatureSpan">mori.mergeWith.</span>d (a, b)](#apidoc.element.mori.mergeWith.d)
1.  [function <span class="apidocSignatureSpan">mori.mergeWith.</span>f (a)](#apidoc.element.mori.mergeWith.f)
1.  number <span class="apidocSignatureSpan">mori.mergeWith.</span>i

#### [module mori.mutable](#apidoc.module.mori.mutable)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>assoc (a, d, e, f)](#apidoc.element.mori.mutable.assoc)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>conj (b, e, f)](#apidoc.element.mori.mutable.conj)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>disj (a, d, e)](#apidoc.element.mori.mutable.disj)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>dissoc (a, d, e)](#apidoc.element.mori.mutable.dissoc)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>freeze (a)](#apidoc.element.mori.mutable.freeze)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>pop (a)](#apidoc.element.mori.mutable.pop)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>thaw (a)](#apidoc.element.mori.mutable.thaw)

#### [module mori.mutable.assoc](#apidoc.module.mori.mutable.assoc)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>assoc (a, d, e, f)](#apidoc.element.mori.mutable.assoc.assoc)
1.  [function <span class="apidocSignatureSpan">mori.mutable.assoc.</span>c (a, b, e)](#apidoc.element.mori.mutable.assoc.c)
1.  [function <span class="apidocSignatureSpan">mori.mutable.assoc.</span>d (a, c, d, h)](#apidoc.element.mori.mutable.assoc.d)
1.  [function <span class="apidocSignatureSpan">mori.mutable.assoc.</span>f (a)](#apidoc.element.mori.mutable.assoc.f)
1.  [function <span class="apidocSignatureSpan">mori.mutable.assoc.</span>f3 (a, b, e)](#apidoc.element.mori.mutable.assoc.f3)
1.  number <span class="apidocSignatureSpan">mori.mutable.assoc.</span>i
1.  object <span class="apidocSignatureSpan">mori.mutable.assoc.</span>fn

#### [module mori.mutable.conj](#apidoc.module.mori.mutable.conj)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>conj (b, e, f)](#apidoc.element.mori.mutable.conj.conj)
1.  [function <span class="apidocSignatureSpan">mori.mutable.conj.</span>a (a, b)](#apidoc.element.mori.mutable.conj.a)
1.  [function <span class="apidocSignatureSpan">mori.mutable.conj.</span>b (a)](#apidoc.element.mori.mutable.conj.b)
1.  [function <span class="apidocSignatureSpan">mori.mutable.conj.</span>d (a, c, d)](#apidoc.element.mori.mutable.conj.d)
1.  [function <span class="apidocSignatureSpan">mori.mutable.conj.</span>f (a)](#apidoc.element.mori.mutable.conj.f)
1.  [function <span class="apidocSignatureSpan">mori.mutable.conj.</span>f0 ()](#apidoc.element.mori.mutable.conj.f0)
1.  [function <span class="apidocSignatureSpan">mori.mutable.conj.</span>f1 (a)](#apidoc.element.mori.mutable.conj.f1)
1.  [function <span class="apidocSignatureSpan">mori.mutable.conj.</span>f2 (a, b)](#apidoc.element.mori.mutable.conj.f2)
1.  [function <span class="apidocSignatureSpan">mori.mutable.conj.</span>l ()](#apidoc.element.mori.mutable.conj.l)
1.  number <span class="apidocSignatureSpan">mori.mutable.conj.</span>i
1.  object <span class="apidocSignatureSpan">mori.mutable.conj.</span>fn

#### [module mori.mutable.disj](#apidoc.module.mori.mutable.disj)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>disj (a, d, e)](#apidoc.element.mori.mutable.disj.disj)
1.  [function <span class="apidocSignatureSpan">mori.mutable.disj.</span>a (a, b)](#apidoc.element.mori.mutable.disj.a)
1.  [function <span class="apidocSignatureSpan">mori.mutable.disj.</span>d (a, c, d)](#apidoc.element.mori.mutable.disj.d)
1.  [function <span class="apidocSignatureSpan">mori.mutable.disj.</span>f (a)](#apidoc.element.mori.mutable.disj.f)
1.  [function <span class="apidocSignatureSpan">mori.mutable.disj.</span>f2 (a, b)](#apidoc.element.mori.mutable.disj.f2)
1.  number <span class="apidocSignatureSpan">mori.mutable.disj.</span>i
1.  object <span class="apidocSignatureSpan">mori.mutable.disj.</span>fn

#### [module mori.mutable.dissoc](#apidoc.module.mori.mutable.dissoc)
1.  [function <span class="apidocSignatureSpan">mori.mutable.</span>dissoc (a, d, e)](#apidoc.element.mori.mutable.dissoc.dissoc)
1.  [function <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>a (a, b)](#apidoc.element.mori.mutable.dissoc.a)
1.  [function <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>d (a, c, d)](#apidoc.element.mori.mutable.dissoc.d)
1.  [function <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>f (a)](#apidoc.element.mori.mutable.dissoc.f)
1.  [function <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>f2 (a, b)](#apidoc.element.mori.mutable.dissoc.f2)
1.  number <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>i
1.  object <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>fn

#### [module mori.notEquals](#apidoc.module.mori.notEquals)
1.  [function <span class="apidocSignatureSpan">mori.</span>notEquals (b, e, f)](#apidoc.element.mori.notEquals.notEquals)
1.  [function <span class="apidocSignatureSpan">mori.notEquals.</span>a (a, b)](#apidoc.element.mori.notEquals.a)
1.  [function <span class="apidocSignatureSpan">mori.notEquals.</span>b ()](#apidoc.element.mori.notEquals.b)
1.  [function <span class="apidocSignatureSpan">mori.notEquals.</span>d (a, c, d)](#apidoc.element.mori.notEquals.d)
1.  [function <span class="apidocSignatureSpan">mori.notEquals.</span>f (a)](#apidoc.element.mori.notEquals.f)
1.  [function <span class="apidocSignatureSpan">mori.notEquals.</span>f1 ()](#apidoc.element.mori.notEquals.f1)
1.  [function <span class="apidocSignatureSpan">mori.notEquals.</span>f2 (a, b)](#apidoc.element.mori.notEquals.f2)
1.  number <span class="apidocSignatureSpan">mori.notEquals.</span>i
1.  object <span class="apidocSignatureSpan">mori.notEquals.</span>fn

#### [module mori.nth](#apidoc.module.mori.nth)
1.  [function <span class="apidocSignatureSpan">mori.</span>nth (c, e, f)](#apidoc.element.mori.nth.nth)
1.  [function <span class="apidocSignatureSpan">mori.nth.</span>a (a, b)](#apidoc.element.mori.nth.a)
1.  [function <span class="apidocSignatureSpan">mori.nth.</span>c (a, b, c)](#apidoc.element.mori.nth.c)
1.  [function <span class="apidocSignatureSpan">mori.nth.</span>f2 (a, b)](#apidoc.element.mori.nth.f2)
1.  [function <span class="apidocSignatureSpan">mori.nth.</span>f3 (a, b, c)](#apidoc.element.mori.nth.f3)

#### [module mori.partial](#apidoc.module.mori.partial)
1.  [function <span class="apidocSignatureSpan">mori.</span>partial (d, g, h, l, m)](#apidoc.element.mori.partial.partial)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>a (a, b)](#apidoc.element.mori.partial.a)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>b (a)](#apidoc.element.mori.partial.b)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>c (a, b, c)](#apidoc.element.mori.partial.c)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>d (a, c, d, e, f)](#apidoc.element.mori.partial.d)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>f (a)](#apidoc.element.mori.partial.f)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>f1 (a)](#apidoc.element.mori.partial.f1)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>f2 (a, b)](#apidoc.element.mori.partial.f2)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>f3 (a, b, c)](#apidoc.element.mori.partial.f3)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>f4 (a, b, c, d)](#apidoc.element.mori.partial.f4)
1.  [function <span class="apidocSignatureSpan">mori.partial.</span>n (a, b, c, d)](#apidoc.element.mori.partial.n)
1.  number <span class="apidocSignatureSpan">mori.partial.</span>i
1.  object <span class="apidocSignatureSpan">mori.partial.</span>fn

#### [module mori.partition](#apidoc.module.mori.partition)
1.  [function <span class="apidocSignatureSpan">mori.</span>partition (d, f, g, h)](#apidoc.element.mori.partition.partition)
1.  [function <span class="apidocSignatureSpan">mori.partition.</span>a (a, b)](#apidoc.element.mori.partition.a)
1.  [function <span class="apidocSignatureSpan">mori.partition.</span>c (a, b, c)](#apidoc.element.mori.partition.c)
1.  [function <span class="apidocSignatureSpan">mori.partition.</span>f2 (a, b)](#apidoc.element.mori.partition.f2)
1.  [function <span class="apidocSignatureSpan">mori.partition.</span>f3 (a, b, c)](#apidoc.element.mori.partition.f3)
1.  [function <span class="apidocSignatureSpan">mori.partition.</span>f4 (a, b, c, h)](#apidoc.element.mori.partition.f4)
1.  [function <span class="apidocSignatureSpan">mori.partition.</span>n (a, b, c, h)](#apidoc.element.mori.partition.n)

#### [module mori.partitionAll](#apidoc.module.mori.partitionAll)
1.  [function <span class="apidocSignatureSpan">mori.</span>partitionAll (d, f, g)](#apidoc.element.mori.partitionAll.partitionAll)
1.  [function <span class="apidocSignatureSpan">mori.partitionAll.</span>a (a, b)](#apidoc.element.mori.partitionAll.a)
1.  [function <span class="apidocSignatureSpan">mori.partitionAll.</span>b (a)](#apidoc.element.mori.partitionAll.b)
1.  [function <span class="apidocSignatureSpan">mori.partitionAll.</span>c (a, b, c)](#apidoc.element.mori.partitionAll.c)
1.  [function <span class="apidocSignatureSpan">mori.partitionAll.</span>f1 (a)](#apidoc.element.mori.partitionAll.f1)
1.  [function <span class="apidocSignatureSpan">mori.partitionAll.</span>f2 (a, b)](#apidoc.element.mori.partitionAll.f2)
1.  [function <span class="apidocSignatureSpan">mori.partitionAll.</span>f3 (a, b, c)](#apidoc.element.mori.partitionAll.f3)

#### [module mori.partitionBy](#apidoc.module.mori.partitionBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>partitionBy (c, e)](#apidoc.element.mori.partitionBy.partitionBy)
1.  [function <span class="apidocSignatureSpan">mori.partitionBy.</span>a (a, b)](#apidoc.element.mori.partitionBy.a)
1.  [function <span class="apidocSignatureSpan">mori.partitionBy.</span>b (a)](#apidoc.element.mori.partitionBy.b)
1.  [function <span class="apidocSignatureSpan">mori.partitionBy.</span>f1 (a)](#apidoc.element.mori.partitionBy.f1)
1.  [function <span class="apidocSignatureSpan">mori.partitionBy.</span>f2 (a, b)](#apidoc.element.mori.partitionBy.f2)

#### [module mori.pipeline](#apidoc.module.mori.pipeline)
1.  [function <span class="apidocSignatureSpan">mori.</span>pipeline (a)](#apidoc.element.mori.pipeline.pipeline)
1.  [function <span class="apidocSignatureSpan">mori.pipeline.</span>d (a)](#apidoc.element.mori.pipeline.d)
1.  [function <span class="apidocSignatureSpan">mori.pipeline.</span>f (a)](#apidoc.element.mori.pipeline.f)
1.  number <span class="apidocSignatureSpan">mori.pipeline.</span>i

#### [module mori.primSeq](#apidoc.module.mori.primSeq)
1.  [function <span class="apidocSignatureSpan">mori.</span>primSeq (c, e)](#apidoc.element.mori.primSeq.primSeq)
1.  [function <span class="apidocSignatureSpan">mori.primSeq.</span>a (a, b)](#apidoc.element.mori.primSeq.a)
1.  [function <span class="apidocSignatureSpan">mori.primSeq.</span>b (a)](#apidoc.element.mori.primSeq.b)
1.  [function <span class="apidocSignatureSpan">mori.primSeq.</span>f1 (a)](#apidoc.element.mori.primSeq.f1)
1.  [function <span class="apidocSignatureSpan">mori.primSeq.</span>f2 (a, b)](#apidoc.element.mori.primSeq.f2)

#### [module mori.queue](#apidoc.module.mori.queue)
1.  [function <span class="apidocSignatureSpan">mori.</span>queue (a)](#apidoc.element.mori.queue.queue)
1.  [function <span class="apidocSignatureSpan">mori.queue.</span>d (a)](#apidoc.element.mori.queue.d)
1.  [function <span class="apidocSignatureSpan">mori.queue.</span>f (a)](#apidoc.element.mori.queue.f)
1.  number <span class="apidocSignatureSpan">mori.queue.</span>i

#### [module mori.range](#apidoc.module.mori.range)
1.  [function <span class="apidocSignatureSpan">mori.</span>range (e, g, h)](#apidoc.element.mori.range.range)
1.  [function <span class="apidocSignatureSpan">mori.range.</span>a (a, b)](#apidoc.element.mori.range.a)
1.  [function <span class="apidocSignatureSpan">mori.range.</span>b (a)](#apidoc.element.mori.range.b)
1.  [function <span class="apidocSignatureSpan">mori.range.</span>c (a, b, c)](#apidoc.element.mori.range.c)
1.  [function <span class="apidocSignatureSpan">mori.range.</span>f0 ()](#apidoc.element.mori.range.f0)
1.  [function <span class="apidocSignatureSpan">mori.range.</span>f1 (a)](#apidoc.element.mori.range.f1)
1.  [function <span class="apidocSignatureSpan">mori.range.</span>f2 (a, b)](#apidoc.element.mori.range.f2)
1.  [function <span class="apidocSignatureSpan">mori.range.</span>f3 (a, b, c)](#apidoc.element.mori.range.f3)
1.  [function <span class="apidocSignatureSpan">mori.range.</span>l ()](#apidoc.element.mori.range.l)

#### [module mori.reduce](#apidoc.module.mori.reduce)
1.  [function <span class="apidocSignatureSpan">mori.</span>reduce (c, e, f)](#apidoc.element.mori.reduce.reduce)
1.  [function <span class="apidocSignatureSpan">mori.reduce.</span>a (a, b)](#apidoc.element.mori.reduce.a)
1.  [function <span class="apidocSignatureSpan">mori.reduce.</span>c (a, b, c)](#apidoc.element.mori.reduce.c)
1.  [function <span class="apidocSignatureSpan">mori.reduce.</span>f2 (a, b)](#apidoc.element.mori.reduce.f2)
1.  [function <span class="apidocSignatureSpan">mori.reduce.</span>f3 (a, b, c)](#apidoc.element.mori.reduce.f3)

#### [module mori.remove](#apidoc.module.mori.remove)
1.  [function <span class="apidocSignatureSpan">mori.</span>remove (c, e)](#apidoc.element.mori.remove.remove)
1.  [function <span class="apidocSignatureSpan">mori.remove.</span>a (a, b)](#apidoc.element.mori.remove.a)
1.  [function <span class="apidocSignatureSpan">mori.remove.</span>b (a)](#apidoc.element.mori.remove.b)
1.  [function <span class="apidocSignatureSpan">mori.remove.</span>f1 (a)](#apidoc.element.mori.remove.f1)
1.  [function <span class="apidocSignatureSpan">mori.remove.</span>f2 (a, b)](#apidoc.element.mori.remove.f2)

#### [module mori.repeat](#apidoc.module.mori.repeat)
1.  [function <span class="apidocSignatureSpan">mori.</span>repeat (c, e)](#apidoc.element.mori.repeat.repeat)
1.  [function <span class="apidocSignatureSpan">mori.repeat.</span>a (a, b)](#apidoc.element.mori.repeat.a)
1.  [function <span class="apidocSignatureSpan">mori.repeat.</span>b (a)](#apidoc.element.mori.repeat.b)
1.  [function <span class="apidocSignatureSpan">mori.repeat.</span>f1 (a)](#apidoc.element.mori.repeat.f1)
1.  [function <span class="apidocSignatureSpan">mori.repeat.</span>f2 (a, b)](#apidoc.element.mori.repeat.f2)

#### [module mori.repeatedly](#apidoc.module.mori.repeatedly)
1.  [function <span class="apidocSignatureSpan">mori.</span>repeatedly (c, e)](#apidoc.element.mori.repeatedly.repeatedly)
1.  [function <span class="apidocSignatureSpan">mori.repeatedly.</span>a (a, b)](#apidoc.element.mori.repeatedly.a)
1.  [function <span class="apidocSignatureSpan">mori.repeatedly.</span>b (a)](#apidoc.element.mori.repeatedly.b)
1.  [function <span class="apidocSignatureSpan">mori.repeatedly.</span>f1 (a)](#apidoc.element.mori.repeatedly.f1)
1.  [function <span class="apidocSignatureSpan">mori.repeatedly.</span>f2 (a, b)](#apidoc.element.mori.repeatedly.f2)

#### [module mori.sequence](#apidoc.module.mori.sequence)
1.  [function <span class="apidocSignatureSpan">mori.</span>sequence (b, e, f)](#apidoc.element.mori.sequence.sequence)
1.  [function <span class="apidocSignatureSpan">mori.sequence.</span>a (a, b)](#apidoc.element.mori.sequence.a)
1.  [function <span class="apidocSignatureSpan">mori.sequence.</span>b (a)](#apidoc.element.mori.sequence.b)
1.  [function <span class="apidocSignatureSpan">mori.sequence.</span>d (a, c, d)](#apidoc.element.mori.sequence.d)
1.  [function <span class="apidocSignatureSpan">mori.sequence.</span>f (a)](#apidoc.element.mori.sequence.f)
1.  [function <span class="apidocSignatureSpan">mori.sequence.</span>f1 (a)](#apidoc.element.mori.sequence.f1)
1.  [function <span class="apidocSignatureSpan">mori.sequence.</span>f2 (a, b)](#apidoc.element.mori.sequence.f2)
1.  number <span class="apidocSignatureSpan">mori.sequence.</span>i
1.  object <span class="apidocSignatureSpan">mori.sequence.</span>fn

#### [module mori.sort](#apidoc.module.mori.sort)
1.  [function <span class="apidocSignatureSpan">mori.</span>sort (c, e)](#apidoc.element.mori.sort.sort)
1.  [function <span class="apidocSignatureSpan">mori.sort.</span>a (a, b)](#apidoc.element.mori.sort.a)
1.  [function <span class="apidocSignatureSpan">mori.sort.</span>b (a)](#apidoc.element.mori.sort.b)
1.  [function <span class="apidocSignatureSpan">mori.sort.</span>f1 (a)](#apidoc.element.mori.sort.f1)
1.  [function <span class="apidocSignatureSpan">mori.sort.</span>f2 (a, b)](#apidoc.element.mori.sort.f2)

#### [module mori.sortBy](#apidoc.module.mori.sortBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortBy (c, e, f)](#apidoc.element.mori.sortBy.sortBy)
1.  [function <span class="apidocSignatureSpan">mori.sortBy.</span>a (a, b)](#apidoc.element.mori.sortBy.a)
1.  [function <span class="apidocSignatureSpan">mori.sortBy.</span>c (a, b, c)](#apidoc.element.mori.sortBy.c)
1.  [function <span class="apidocSignatureSpan">mori.sortBy.</span>f2 (a, b)](#apidoc.element.mori.sortBy.f2)
1.  [function <span class="apidocSignatureSpan">mori.sortBy.</span>f3 (a, b, c)](#apidoc.element.mori.sortBy.f3)

#### [module mori.sortedMap](#apidoc.module.mori.sortedMap)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortedMap (a)](#apidoc.element.mori.sortedMap.sortedMap)
1.  [function <span class="apidocSignatureSpan">mori.sortedMap.</span>d (a)](#apidoc.element.mori.sortedMap.d)
1.  [function <span class="apidocSignatureSpan">mori.sortedMap.</span>f (a)](#apidoc.element.mori.sortedMap.f)
1.  number <span class="apidocSignatureSpan">mori.sortedMap.</span>i

#### [module mori.sortedMapBy](#apidoc.module.mori.sortedMapBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortedMapBy (a, d)](#apidoc.element.mori.sortedMapBy.sortedMapBy)
1.  [function <span class="apidocSignatureSpan">mori.sortedMapBy.</span>d (a, b)](#apidoc.element.mori.sortedMapBy.d)
1.  [function <span class="apidocSignatureSpan">mori.sortedMapBy.</span>f (a)](#apidoc.element.mori.sortedMapBy.f)
1.  number <span class="apidocSignatureSpan">mori.sortedMapBy.</span>i

#### [module mori.sortedSet](#apidoc.module.mori.sortedSet)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortedSet (a)](#apidoc.element.mori.sortedSet.sortedSet)
1.  [function <span class="apidocSignatureSpan">mori.sortedSet.</span>d (a)](#apidoc.element.mori.sortedSet.d)
1.  [function <span class="apidocSignatureSpan">mori.sortedSet.</span>f (a)](#apidoc.element.mori.sortedSet.f)
1.  number <span class="apidocSignatureSpan">mori.sortedSet.</span>i

#### [module mori.sortedSetBy](#apidoc.module.mori.sortedSetBy)
1.  [function <span class="apidocSignatureSpan">mori.</span>sortedSetBy (a, d)](#apidoc.element.mori.sortedSetBy.sortedSetBy)
1.  [function <span class="apidocSignatureSpan">mori.sortedSetBy.</span>d (a, b)](#apidoc.element.mori.sortedSetBy.d)
1.  [function <span class="apidocSignatureSpan">mori.sortedSetBy.</span>f (a)](#apidoc.element.mori.sortedSetBy.f)
1.  number <span class="apidocSignatureSpan">mori.sortedSetBy.</span>i

#### [module mori.subseq](#apidoc.module.mori.subseq)
1.  [function <span class="apidocSignatureSpan">mori.</span>subseq (c, e, f, g, h)](#apidoc.element.mori.subseq.subseq)
1.  [function <span class="apidocSignatureSpan">mori.subseq.</span>c (a, b, c)](#apidoc.element.mori.subseq.c)
1.  [function <span class="apidocSignatureSpan">mori.subseq.</span>f3 (a, b, c)](#apidoc.element.mori.subseq.f3)
1.  [function <span class="apidocSignatureSpan">mori.subseq.</span>f5 (a, b, c, g, h)](#apidoc.element.mori.subseq.f5)
1.  [function <span class="apidocSignatureSpan">mori.subseq.</span>r (a, b, c, g, h)](#apidoc.element.mori.subseq.r)

#### [module mori.subvec](#apidoc.module.mori.subvec)
1.  [function <span class="apidocSignatureSpan">mori.</span>subvec (c, e, f)](#apidoc.element.mori.subvec.subvec)
1.  [function <span class="apidocSignatureSpan">mori.subvec.</span>a (a, b)](#apidoc.element.mori.subvec.a)
1.  [function <span class="apidocSignatureSpan">mori.subvec.</span>c (a, b, c)](#apidoc.element.mori.subvec.c)
1.  [function <span class="apidocSignatureSpan">mori.subvec.</span>f2 (a, b)](#apidoc.element.mori.subvec.f2)
1.  [function <span class="apidocSignatureSpan">mori.subvec.</span>f3 (a, b, c)](#apidoc.element.mori.subvec.f3)

#### [module mori.sum](#apidoc.module.mori.sum)
1.  [function <span class="apidocSignatureSpan">mori.</span>sum (a, d, e)](#apidoc.element.mori.sum.sum)
1.  [function <span class="apidocSignatureSpan">mori.sum.</span>a (a, b)](#apidoc.element.mori.sum.a)
1.  [function <span class="apidocSignatureSpan">mori.sum.</span>b (a)](#apidoc.element.mori.sum.b)
1.  [function <span class="apidocSignatureSpan">mori.sum.</span>d (b, c, d)](#apidoc.element.mori.sum.d)
1.  [function <span class="apidocSignatureSpan">mori.sum.</span>f (a)](#apidoc.element.mori.sum.f)
1.  [function <span class="apidocSignatureSpan">mori.sum.</span>f0 ()](#apidoc.element.mori.sum.f0)
1.  [function <span class="apidocSignatureSpan">mori.sum.</span>f1 (a)](#apidoc.element.mori.sum.f1)
1.  [function <span class="apidocSignatureSpan">mori.sum.</span>f2 (a, b)](#apidoc.element.mori.sum.f2)
1.  [function <span class="apidocSignatureSpan">mori.sum.</span>l ()](#apidoc.element.mori.sum.l)
1.  number <span class="apidocSignatureSpan">mori.sum.</span>i
1.  object <span class="apidocSignatureSpan">mori.sum.</span>fn

#### [module mori.symbol](#apidoc.module.mori.symbol)
1.  [function <span class="apidocSignatureSpan">mori.</span>symbol (c, e)](#apidoc.element.mori.symbol.symbol)
1.  [function <span class="apidocSignatureSpan">mori.symbol.</span>a (a, b)](#apidoc.element.mori.symbol.a)
1.  [function <span class="apidocSignatureSpan">mori.symbol.</span>b (a)](#apidoc.element.mori.symbol.b)
1.  [function <span class="apidocSignatureSpan">mori.symbol.</span>f1 (a)](#apidoc.element.mori.symbol.f1)
1.  [function <span class="apidocSignatureSpan">mori.symbol.</span>f2 (a, b)](#apidoc.element.mori.symbol.f2)

#### [module mori.take](#apidoc.module.mori.take)
1.  [function <span class="apidocSignatureSpan">mori.</span>take (c, e)](#apidoc.element.mori.take.take)
1.  [function <span class="apidocSignatureSpan">mori.take.</span>a (a, b)](#apidoc.element.mori.take.a)
1.  [function <span class="apidocSignatureSpan">mori.take.</span>b (a)](#apidoc.element.mori.take.b)
1.  [function <span class="apidocSignatureSpan">mori.take.</span>f1 (a)](#apidoc.element.mori.take.f1)
1.  [function <span class="apidocSignatureSpan">mori.take.</span>f2 (a, b)](#apidoc.element.mori.take.f2)

#### [module mori.takeNth](#apidoc.module.mori.takeNth)
1.  [function <span class="apidocSignatureSpan">mori.</span>takeNth (c, e)](#apidoc.element.mori.takeNth.takeNth)
1.  [function <span class="apidocSignatureSpan">mori.takeNth.</span>a (a, b)](#apidoc.element.mori.takeNth.a)
1.  [function <span class="apidocSignatureSpan">mori.takeNth.</span>b (a)](#apidoc.element.mori.takeNth.b)
1.  [function <span class="apidocSignatureSpan">mori.takeNth.</span>f1 (a)](#apidoc.element.mori.takeNth.f1)
1.  [function <span class="apidocSignatureSpan">mori.takeNth.</span>f2 (a, b)](#apidoc.element.mori.takeNth.f2)

#### [module mori.takeWhile](#apidoc.module.mori.takeWhile)
1.  [function <span class="apidocSignatureSpan">mori.</span>takeWhile (c, e)](#apidoc.element.mori.takeWhile.takeWhile)
1.  [function <span class="apidocSignatureSpan">mori.takeWhile.</span>a (a, b)](#apidoc.element.mori.takeWhile.a)
1.  [function <span class="apidocSignatureSpan">mori.takeWhile.</span>b (a)](#apidoc.element.mori.takeWhile.b)
1.  [function <span class="apidocSignatureSpan">mori.takeWhile.</span>f1 (a)](#apidoc.element.mori.takeWhile.f1)
1.  [function <span class="apidocSignatureSpan">mori.takeWhile.</span>f2 (a, b)](#apidoc.element.mori.takeWhile.f2)

#### [module mori.toClj](#apidoc.module.mori.toClj)
1.  [function <span class="apidocSignatureSpan">mori.</span>toClj (c, e)](#apidoc.element.mori.toClj.toClj)
1.  [function <span class="apidocSignatureSpan">mori.toClj.</span>a (a, b)](#apidoc.element.mori.toClj.a)
1.  [function <span class="apidocSignatureSpan">mori.toClj.</span>b (a)](#apidoc.element.mori.toClj.b)

#### [module mori.transduce](#apidoc.module.mori.transduce)
1.  [function <span class="apidocSignatureSpan">mori.</span>transduce (c, e, f, g)](#apidoc.element.mori.transduce.transduce)
1.  [function <span class="apidocSignatureSpan">mori.transduce.</span>c (a, b, f)](#apidoc.element.mori.transduce.c)
1.  [function <span class="apidocSignatureSpan">mori.transduce.</span>f3 (a, b, f)](#apidoc.element.mori.transduce.f3)
1.  [function <span class="apidocSignatureSpan">mori.transduce.</span>f4 (a, b, c, g)](#apidoc.element.mori.transduce.f4)
1.  [function <span class="apidocSignatureSpan">mori.transduce.</span>n (a, b, c, g)](#apidoc.element.mori.transduce.n)

#### [module mori.union](#apidoc.module.mori.union)
1.  [function <span class="apidocSignatureSpan">mori.</span>union (b, e, f)](#apidoc.element.mori.union.union)
1.  [function <span class="apidocSignatureSpan">mori.union.</span>a (a, b)](#apidoc.element.mori.union.a)
1.  [function <span class="apidocSignatureSpan">mori.union.</span>b (a)](#apidoc.element.mori.union.b)
1.  [function <span class="apidocSignatureSpan">mori.union.</span>d (a, c, d)](#apidoc.element.mori.union.d)
1.  [function <span class="apidocSignatureSpan">mori.union.</span>f (a)](#apidoc.element.mori.union.f)
1.  [function <span class="apidocSignatureSpan">mori.union.</span>f0 ()](#apidoc.element.mori.union.f0)
1.  [function <span class="apidocSignatureSpan">mori.union.</span>f1 (a)](#apidoc.element.mori.union.f1)
1.  [function <span class="apidocSignatureSpan">mori.union.</span>f2 (a, b)](#apidoc.element.mori.union.f2)
1.  [function <span class="apidocSignatureSpan">mori.union.</span>l ()](#apidoc.element.mori.union.l)
1.  number <span class="apidocSignatureSpan">mori.union.</span>i
1.  object <span class="apidocSignatureSpan">mori.union.</span>fn

#### [module mori.updateIn](#apidoc.module.mori.updateIn)
1.  [function <span class="apidocSignatureSpan">mori.</span>updateIn (e, h, l, m, p, q, s)](#apidoc.element.mori.updateIn.updateIn)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>P (a, b, c, d, f, q)](#apidoc.element.mori.updateIn.P)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>c (a, b, c)](#apidoc.element.mori.updateIn.c)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>d (a, c, d, f, g, h, v)](#apidoc.element.mori.updateIn.d)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>f (a)](#apidoc.element.mori.updateIn.f)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>f3 (a, b, c)](#apidoc.element.mori.updateIn.f3)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>f4 (a, b, c, d)](#apidoc.element.mori.updateIn.f4)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>f5 (a, b, c, d, f)](#apidoc.element.mori.updateIn.f5)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>f6 (a, b, c, d, f, q)](#apidoc.element.mori.updateIn.f6)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>n (a, b, c, d)](#apidoc.element.mori.updateIn.n)
1.  [function <span class="apidocSignatureSpan">mori.updateIn.</span>r (a, b, c, d, f)](#apidoc.element.mori.updateIn.r)
1.  number <span class="apidocSignatureSpan">mori.updateIn.</span>i
1.  object <span class="apidocSignatureSpan">mori.updateIn.</span>fn

#### [module mori.varyMeta](#apidoc.module.mori.varyMeta)
1.  [function <span class="apidocSignatureSpan">mori.</span>varyMeta (f, l, m, p, q, s, u)](#apidoc.element.mori.varyMeta.varyMeta)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>P (a, b, c, d, e, f)](#apidoc.element.mori.varyMeta.P)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>a (a, b)](#apidoc.element.mori.varyMeta.a)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>c (a, b, c)](#apidoc.element.mori.varyMeta.c)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>d (a, c, d, e, f, g, h)](#apidoc.element.mori.varyMeta.d)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>f (a)](#apidoc.element.mori.varyMeta.f)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>f2 (a, b)](#apidoc.element.mori.varyMeta.f2)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>f3 (a, b, c)](#apidoc.element.mori.varyMeta.f3)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>f4 (a, b, c, d)](#apidoc.element.mori.varyMeta.f4)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>f5 (a, b, c, d, e)](#apidoc.element.mori.varyMeta.f5)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>f6 (a, b, c, d, e, f)](#apidoc.element.mori.varyMeta.f6)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>n (a, b, c, d)](#apidoc.element.mori.varyMeta.n)
1.  [function <span class="apidocSignatureSpan">mori.varyMeta.</span>r (a, b, c, d, e)](#apidoc.element.mori.varyMeta.r)
1.  number <span class="apidocSignatureSpan">mori.varyMeta.</span>i
1.  object <span class="apidocSignatureSpan">mori.varyMeta.</span>fn

#### [module mori.vector](#apidoc.module.mori.vector)
1.  [function <span class="apidocSignatureSpan">mori.</span>vector (a)](#apidoc.element.mori.vector.vector)
1.  [function <span class="apidocSignatureSpan">mori.vector.</span>d (a)](#apidoc.element.mori.vector.d)
1.  [function <span class="apidocSignatureSpan">mori.vector.</span>f (a)](#apidoc.element.mori.vector.f)
1.  number <span class="apidocSignatureSpan">mori.vector.</span>i



# <a name="apidoc.module.mori"></a>[module mori](#apidoc.module.mori)

#### <a name="apidoc.element.mori.alterMeta"></a>[function <span class="apidocSignatureSpan">mori.</span>alterMeta (a, d, e)](#apidoc.element.mori.alterMeta)
- description and source-code
```javascript
function a(a, d, e){var f=null;if(2<arguments.length){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;
f=new F(g,0)}return b.call(this,a,d,f)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply"></a>[function <span class="apidocSignatureSpan">mori.</span>apply (e, h, l, m, p, q)](#apidoc.element.mori.apply)
- description and source-code
```javascript
apply = function (e, h, l, m, p, q){switch(arguments.length){case 2:return d.call(this,e,h);case 3:return c.call(this,
e,h,l);case 4:return b.call(this,e,h,l,m);case 5:return a.call(this,e,h,l,m,p);default:var s=null;if(5<arguments.length){for(var
 s=0,u=Array(arguments.length-5);s<u.length;)u[s]=arguments[s+5],++s;s=new F(u,0)}return f.d(e,h,l,m,p,s)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.assoc"></a>[function <span class="apidocSignatureSpan">mori.</span>assoc (b, e, f, g)](#apidoc.element.mori.assoc)
- description and source-code
```javascript
assoc = function (b, e, f, g){switch(arguments.length){case 3:return a.call(this,b,e,f);default:var h=null;if(3<arguments.length){for(var h
=0,l=Array(arguments.length-3);h<l.length;)l[h]=arguments[h+3],++h;h=new F(l,0)}return c.d(b,e,f,h)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.assocIn"></a>[function <span class="apidocSignatureSpan">mori.</span>assocIn (b, c, d)](#apidoc.element.mori.assocIn)
- description and source-code
```javascript
function Yh(b, c, d){var e=R.c(c,0,null);return(c=Ed(c))?Rc.c(b,e,Yh(S.a(b,e),c,d)):Rc.c(b,e,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp"></a>[function <span class="apidocSignatureSpan">mori.</span>comp (c, f, g, h)](#apidoc.element.mori.comp)
- description and source-code
```javascript
comp = function (c, f, g, h){switch(arguments.length){case 0:return ud;case 1:return c;case 2:return b.call(this,c,f);case 3:return a.call
(this,c,f,g);default:var l=null;if(3<arguments.length){for(var l=0,m=Array(arguments.length-3);l<m.length;)m[l]=arguments[l+3],++
l;l=new F(m,0)}return d.d(c,f,g,l)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
  var s = new Date();
  f();
  console.log(((new Date())-s)+"ms");
}

// ~190ms V8 version 3.29.80 MBP 2.26ghz
time(function() {
  var xf = m.comp(m.map(m.inc), m.map(m.inc), m.map(m.inc));
  return m.transduce(xf, m.completing(m.sum), 0, v);
}, 10);

// ~440ms
time(function() {
  return a.map(m.inc).map(m.inc).map(m.inc).reduce(function(a,b){return a+b;}, 0);
}, 10);
...
```

#### <a name="apidoc.element.mori.compare"></a>[function <span class="apidocSignatureSpan">mori.</span>compare (a, b)](#apidoc.element.mori.compare)
- description and source-code
```javascript
function od(a, b){if(a===b)return 0;if(null==a)return-1;if(null==b)return 1;if(Ba(a)===Ba(b))return a&&(a.q&2048||a.sb)?a.tb(null
,b):ha(a,b);throw Error("compare on non-nil objects of different types");}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.completing"></a>[function <span class="apidocSignatureSpan">mori.</span>completing (c, e)](#apidoc.element.mori.completing)
- description and source-code
```javascript
completing = function (c, e){switch(arguments.length){case 1:return b.call(this,
c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
  f();
  console.log(((new Date())-s)+"ms");
}

// ~190ms V8 version 3.29.80 MBP 2.26ghz
time(function() {
  var xf = m.comp(m.map(m.inc), m.map(m.inc), m.map(m.inc));
  return m.transduce(xf, m.completing(m.sum), 0, v);
}, 10);

// ~440ms
time(function() {
  return a.map(m.inc).map(m.inc).map(m.inc).reduce(function(a,b){return a+b;}, 0);
}, 10);
'''
...
```

#### <a name="apidoc.element.mori.concat"></a>[function <span class="apidocSignatureSpan">mori.</span>concat (d, g, h)](#apidoc.element.mori.concat)
- description and source-code
```javascript
concat = function (d, g, h){switch(arguments.length){case 0:return c.call(this);case 1:return b.call(this,d);case 2:return a.call(this,d,g);
default:var l=null;if(2<arguments.length){for(var l=0,m=
Array(arguments.length-2);l<m.length;)m[l]=arguments[l+2],++l;l=new F(m,0)}return e.d(d,g,l)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.configure"></a>[function <span class="apidocSignatureSpan">mori.</span>configure (a, b)](#apidoc.element.mori.configure)
- description and source-code
```javascript
configure = function (a, b){switch(a){case "print-length":return la=b;case "print-level":return ma=b;default:throw Error([z("No matching clause
: "),z(a)].join(""));}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.conj"></a>[function <span class="apidocSignatureSpan">mori.</span>conj (b, e, f)](#apidoc.element.mori.conj)
- description and source-code
```javascript
conj = function (b, e, f){switch(arguments.length){case 0:return Mc;case 1:return b;
case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g
]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
var v2 = mori.conj(v1, 4);
v1.toString(); // => '[1 2 3]'
v2.toString(); // => '[1 2 3 4]'
'''

'''javascript
var sum = function(a, b) {
return a + b;
...
```

#### <a name="apidoc.element.mori.cons"></a>[function <span class="apidocSignatureSpan">mori.</span>cons (a, b)](#apidoc.element.mori.cons)
- description and source-code
```javascript
function M(a, b){var c=null==b;return(c?c:b&&(b.j&64||b.jb))?new Ld(null,a,b,null):new Ld(null,a,D(b),null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.constantly"></a>[function <span class="apidocSignatureSpan">mori.</span>constantly (a)](#apidoc.element.mori.constantly)
- description and source-code
```javascript
constantly = function (a){return function(){function b(b){if(0<arguments.length)for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments
[d+0],++d;return a}b.i=0;b.f=function(b){D(b);return a};b.d=function(){return a};return b}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.count"></a>[function <span class="apidocSignatureSpan">mori.</span>count (a)](#apidoc.element.mori.count)
- description and source-code
```javascript
function Q(a){if(null!=a)if(a&&(a.j&2||a.cc))a=a.L(null);else if(a instanceof Array)a=a.length;else if("string"===typeof a)a=a.length
;else if(w(La,a))a=Ma(a);else a:{a=D(a);for(var b=0;;){if(Ec(a)){a=b+Ma(a);break a}a=K(a);b+=1}a=void 0}else a=0;return a}
```
- example usage
```shell
...
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''

### ES6 Map/Set inspired interfaces

All Mori maps and sets support all the non-mutating methods of the
...
```

#### <a name="apidoc.element.mori.curry"></a>[function <span class="apidocSignatureSpan">mori.</span>curry (a, d)](#apidoc.element.mori.curry)
- description and source-code
```javascript
function a(a, d){var e=null;if(1<arguments.length){for(var e=0,f=Array(arguments.length-1);e<f.length;)f[e]=arguments[e+1],++e;e=
new F(f,0)}return b.call(this,a,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dec"></a>[function <span class="apidocSignatureSpan">mori.</span>dec (a)](#apidoc.element.mori.dec)
- description and source-code
```javascript
dec = function (a){return a-1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dedupe"></a>[function <span class="apidocSignatureSpan">mori.</span>dedupe (c)](#apidoc.element.mori.dedupe)
- description and source-code
```javascript
dedupe = function (c){switch(arguments.length){case 0:return b.call(this);case 1:return a.call(this,c)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.difference"></a>[function <span class="apidocSignatureSpan">mori.</span>difference (b, e, f)](#apidoc.element.mori.difference)
- description and source-code
```javascript
difference = function (b, e, f){switch(arguments.length){case 1:return b;case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length
){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid
 arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.disj"></a>[function <span class="apidocSignatureSpan">mori.</span>disj (b, e, f)](#apidoc.element.mori.disj)
- description and source-code
```javascript
disj = function (b, e, f){switch(arguments.length){case 1:return b;case 2:return a.call(this,
b,e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new
 F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dissoc"></a>[function <span class="apidocSignatureSpan">mori.</span>dissoc (b, e, f)](#apidoc.element.mori.dissoc)
- description and source-code
```javascript
dissoc = function (b, e, f){switch(arguments.length){case 1:return b;case 2:return a.call(this,b,e);
default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,
0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.distinct"></a>[function <span class="apidocSignatureSpan">mori.</span>distinct (a)](#apidoc.element.mori.distinct)
- description and source-code
```javascript
distinct = function (a){return function c(a,e){return new V(null,function(){return function(a,d){for(;;){var e=a,l=R.c(e,0,null);if(e=D(e))
if(nd(d,l))l=H(e),e=d,a=l,d=e;else return M(l,c(H(e),Nc.a(d,l)));else return null}}.call(null,a,e)},null,null)}(a,bh)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.drop"></a>[function <span class="apidocSignatureSpan">mori.</span>drop (c, e)](#apidoc.element.mori.drop)
- description and source-code
```javascript
drop = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dropWhile"></a>[function <span class="apidocSignatureSpan">mori.</span>dropWhile (c, e)](#apidoc.element.mori.dropWhile)
- description and source-code
```javascript
dropWhile = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.each"></a>[function <span class="apidocSignatureSpan">mori.</span>each (a, b)](#apidoc.element.mori.each)
- description and source-code
```javascript
each = function (a, b){for(var c=D(a),d=null,e=0,f=0;;)if(f<e){var g=d.Q(null,f);b.b?b.b(g):b.call(null,g);f+=1}else if(c=D(c))fd(c)?(e=
Yb(c),c=Zb(c),d=e,e=Q(e)):(d=g=G(c),b.b?b.b(d):b.call(null,d),c=K(c),d=null,e=0),f=0;else return null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.eduction"></a>[function <span class="apidocSignatureSpan">mori.</span>eduction (a, b)](#apidoc.element.mori.eduction)
- description and source-code
```javascript
eduction = function (a, b){return new Gh(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.empty"></a>[function <span class="apidocSignatureSpan">mori.</span>empty (a)](#apidoc.element.mori.empty)
- description and source-code
```javascript
function Oc(a){return null==a?null:Na(a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.equals"></a>[function <span class="apidocSignatureSpan">mori.</span>equals (b, e, f)](#apidoc.element.mori.equals)
- description and source-code
```javascript
equals = function (b, e, f){switch(arguments.length){case 1:return!0;
case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g
]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.every"></a>[function <span class="apidocSignatureSpan">mori.</span>every (a, b)](#apidoc.element.mori.every)
- description and source-code
```javascript
function Ee(a, b){for(;;){if(null==D(b))return!0;var c;c=G(b);c=a.b?a.b(c):a.call(null,c);if(t(c)){c=a;var d=K(b);a=c;b=d}else return
!1}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.filter"></a>[function <span class="apidocSignatureSpan">mori.</span>filter (c, e)](#apidoc.element.mori.filter)
- description and source-code
```javascript
filter = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.find"></a>[function <span class="apidocSignatureSpan">mori.</span>find (a, b)](#apidoc.element.mori.find)
- description and source-code
```javascript
find = function (a, b){return null!=a&&bd(a)&&nd(a,b)?new W(null,2,5,uf,[b,S.a(a,b)],null):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.first"></a>[function <span class="apidocSignatureSpan">mori.</span>first (a)](#apidoc.element.mori.first)
- description and source-code
```javascript
function G(a){if(null==a)return null;if(a&&(a.j&64||a.jb))return a.N(null);a=D(a);return null==a?null:Va(a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.flatten"></a>[function <span class="apidocSignatureSpan">mori.</span>flatten (a)](#apidoc.element.mori.flatten)
- description and source-code
```javascript
flatten = function (a){return Xe.a(function(a){return!$e(a)},H(Ze(a)))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.fnil"></a>[function <span class="apidocSignatureSpan">mori.</span>fnil (d, f, g, h)](#apidoc.element.mori.fnil)
- description and source-code
```javascript
fnil = function (d, f, g, h){switch(arguments.length){case 2:return c.call(this,d,f);case 3:return b.call(this,d,f,g);case 4:return a.call
(this,d,f,g,h)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.get"></a>[function <span class="apidocSignatureSpan">mori.</span>get (c, e, f)](#apidoc.element.mori.get)
- description and source-code
```javascript
get = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,
c,e,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
return the proposed mutable iterators:

'''javascript
var m = mori;
var h = m.hashMap("foo", 1, "bar", 2);

h.has("foo"); // => true
h.get("foo"); // => 1

var iter = h.keys();
iter.next(); // => {done: false, value: "foo"}
'''

This feature is subject to changes in the ES6 proposal.
...
```

#### <a name="apidoc.element.mori.getIn"></a>[function <span class="apidocSignatureSpan">mori.</span>getIn (c, e, f)](#apidoc.element.mori.getIn)
- description and source-code
```javascript
getIn = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.groupBy"></a>[function <span class="apidocSignatureSpan">mori.</span>groupBy (a, b)](#apidoc.element.mori.groupBy)
- description and source-code
```javascript
groupBy = function (a, b){return ce(A.c(function(b,d){var e=a.b?a.b(d):a.call(null,d);return ee.c(b,e,Nc.a(S.c(b,e,Mc),d))},Ob(Uf),b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gt"></a>[function <span class="apidocSignatureSpan">mori.</span>gt (a, d, e)](#apidoc.element.mori.gt)
- description and source-code
```javascript
gt = function (a, d, e){switch(arguments.length){case 1:return!0;case 2:return a>d;default:var f=null;if(2<arguments.length){for(var f=
0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gte"></a>[function <span class="apidocSignatureSpan">mori.</span>gte (a, d, e)](#apidoc.element.mori.gte)
- description and source-code
```javascript
gte = function (a, d, e){switch(arguments.length){case 1:return!0;case 2:return a>=d;default:var f=null;if(2<arguments.length){for(var f
=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+
2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.hasKey"></a>[function <span class="apidocSignatureSpan">mori.</span>hasKey (a, b)](#apidoc.element.mori.hasKey)
- description and source-code
```javascript
function nd(a, b){return S.c(a,b,jd)===jd?!1:!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.hash"></a>[function <span class="apidocSignatureSpan">mori.</span>hash (a)](#apidoc.element.mori.hash)
- description and source-code
```javascript
function nc(a){a&&(a.j&4194304||a.vc)?a=a.B(null):"number"===typeof a?a=(Math.floor.b?Math.floor.b(a):Math.floor.call(null,a))%2147483647
:!0===a?a=1:!1===a?a=0:"string"===typeof a?(a=mc(a),0!==a&&(a=gc(a),a=hc(0,a),a=ic(a,4))):a=a instanceof Date?a.valueOf():null==
a?0:zb(a);return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.hashMap"></a>[function <span class="apidocSignatureSpan">mori.</span>hashMap (a)](#apidoc.element.mori.hashMap)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,
d)}
```
- example usage
```shell
...
[Set](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set)
interfaces. The main difference with the spec is that key lookup is
based on value not reference. 'keys', 'values', and 'entries' methods
return the proposed mutable iterators:

'''javascript
var m = mori;
var h = m.hashMap("foo", 1, "bar", 2);

h.has("foo"); // => true
h.get("foo"); // => 1

var iter = h.keys();
iter.next(); // => {done: false, value: "foo"}
'''
...
```

#### <a name="apidoc.element.mori.identity"></a>[function <span class="apidocSignatureSpan">mori.</span>identity (a)](#apidoc.element.mori.identity)
- description and source-code
```javascript
function ud(a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.inc"></a>[function <span class="apidocSignatureSpan">mori.</span>inc (a)](#apidoc.element.mori.inc)
- description and source-code
```javascript
inc = function (a){return a+1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.index"></a>[function <span class="apidocSignatureSpan">mori.</span>index (a, b)](#apidoc.element.mori.index)
- description and source-code
```javascript
function Vh(a, b){return A.c(function(a,d){var e=Yg(d,b);return Rc.c(a,e,Nc.a(S.c(a,e,bh),d))},Uf,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.interleave"></a>[function <span class="apidocSignatureSpan">mori.</span>interleave (b, e, f)](#apidoc.element.mori.interleave)
- description and source-code
```javascript
interleave = function (b, e, f){switch(arguments.length){case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length){for(var g=0,h
=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.interpose"></a>[function <span class="apidocSignatureSpan">mori.</span>interpose (a, b)](#apidoc.element.mori.interpose)
- description and source-code
```javascript
interpose = function (a, b){return Qe.a(1,Ue.a(Se.b(a),b))}
```
- example usage
```shell
...
mori.reduce(sum, mori.vector(1, 2, 3, 4)); // => 10
'''

Lazy sequences!

'''javascript
var _ = mori;
_.intoArray(_.interpose("foo", _.vector(1, 2, 3, 4)));
// => [1, "foo", 2, "foo", 3, "foo", 4]
'''

Or if it's more your speed, use it from CoffeeScript!

'''coffeescript
inc = (x) -> x+1
...
```

#### <a name="apidoc.element.mori.intersection"></a>[function <span class="apidocSignatureSpan">mori.</span>intersection (b, e, f)](#apidoc.element.mori.intersection)
- description and source-code
```javascript
intersection = function (b, e, f){switch(arguments.length){case 1:return b;case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length
){for(var g=0,h=Array(arguments.length-
2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.into"></a>[function <span class="apidocSignatureSpan">mori.</span>into (c, e, f)](#apidoc.element.mori.into)
- description and source-code
```javascript
into = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
...
var a = [];

for(var i = 0; i < 1000000; i++) {
  a.push(i);
}

// make it immutable
var v = m.into(m.vector(), a);

function time(f) {
  var s = new Date();
  f();
  console.log(((new Date())-s)+"ms");
}
...
```

#### <a name="apidoc.element.mori.intoArray"></a>[function <span class="apidocSignatureSpan">mori.</span>intoArray (d, c)](#apidoc.element.mori.intoArray)
- description and source-code
```javascript
intoArray = function (d, c){switch(arguments.length){case 1:return b.call(this,d);case 2:return a.call(this,0,c)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
...
You can use it from your projects like so:

'''javascript
var inc = function(n) {
  return n+1;
};

mori.intoArray(mori.map(inc, mori.vector(1,2,3,4,5)));
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
...
```

#### <a name="apidoc.element.mori.isAssociative"></a>[function <span class="apidocSignatureSpan">mori.</span>isAssociative (a)](#apidoc.element.mori.isAssociative)
- description and source-code
```javascript
function bd(a){return a?a.j&512||a.rc?!0:a.j?!1:w(ab,a):w(ab,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isCollection"></a>[function <span class="apidocSignatureSpan">mori.</span>isCollection (a)](#apidoc.element.mori.isCollection)
- description and source-code
```javascript
function $c(a){return null==a?!1:a?a.j&8||a.tc?!0:a.j?!1:w(Qa,a):w(Qa,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isCounted"></a>[function <span class="apidocSignatureSpan">mori.</span>isCounted (a)](#apidoc.element.mori.isCounted)
- description and source-code
```javascript
function Ec(a){return a?a.j&2||a.cc?!0:a.j?!1:w(La,a):w(La,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isEmpty"></a>[function <span class="apidocSignatureSpan">mori.</span>isEmpty (a)](#apidoc.element.mori.isEmpty)
- description and source-code
```javascript
function Yc(a){return null==a||Aa(D(a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isEven"></a>[function <span class="apidocSignatureSpan">mori.</span>isEven (a)](#apidoc.element.mori.isEven)
- description and source-code
```javascript
function Ge(a){if("number"===typeof a&&Aa(isNaN(a))&&Infinity!==a&&parseFloat(a)===parseInt(a,10))return 0===(a&1);throw Error([
z("Argument must be an integer: "),z(a)].join(""));}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isIndexed"></a>[function <span class="apidocSignatureSpan">mori.</span>isIndexed (a)](#apidoc.element.mori.isIndexed)
- description and source-code
```javascript
function Fc(a){return a?a.j&16||a.Qb?!0:a.j?!1:w(Ta,a):w(Ta,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isKeyword"></a>[function <span class="apidocSignatureSpan">mori.</span>isKeyword (a)](#apidoc.element.mori.isKeyword)
- description and source-code
```javascript
isKeyword = function (a){return a instanceof U}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isList"></a>[function <span class="apidocSignatureSpan">mori.</span>isList (a)](#apidoc.element.mori.isList)
- description and source-code
```javascript
isList = function (a){return a?a.j&33554432||a.wc?!0:a.j?!1:w(Eb,a):w(Eb,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isMap"></a>[function <span class="apidocSignatureSpan">mori.</span>isMap (a)](#apidoc.element.mori.isMap)
- description and source-code
```javascript
function dd(a){return null==a?!1:a?a.j&1024||a.ic?!0:a.j?!1:w(db,a):w(db,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isOdd"></a>[function <span class="apidocSignatureSpan">mori.</span>isOdd (a)](#apidoc.element.mori.isOdd)
- description and source-code
```javascript
isOdd = function (a){return!Ge(a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isReduceable"></a>[function <span class="apidocSignatureSpan">mori.</span>isReduceable (a)](#apidoc.element.mori.isReduceable)
- description and source-code
```javascript
isReduceable = function (a){return a?a.j&524288||a.Sb?!0:a.j?!1:w(vb,a):w(vb,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isReversible"></a>[function <span class="apidocSignatureSpan">mori.</span>isReversible (a)](#apidoc.element.mori.isReversible)
- description and source-code
```javascript
function Id(a){return a?a.j&134217728||a.xc?!0:a.j?!1:w(Fb,a):w(Fb,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isSeq"></a>[function <span class="apidocSignatureSpan">mori.</span>isSeq (a)](#apidoc.element.mori.isSeq)
- description and source-code
```javascript
function kd(a){return null==a?!1:a?a.j&64||a.jb?!0:a.j?!1:w(Ua,a):w(Ua,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isSeqable"></a>[function <span class="apidocSignatureSpan">mori.</span>isSeqable (a)](#apidoc.element.mori.isSeqable)
- description and source-code
```javascript
function ld(a){return a?a.j&8388608||a.mc?!0:a.j?!1:w(Bb,a):w(Bb,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isSequential"></a>[function <span class="apidocSignatureSpan">mori.</span>isSequential (a)](#apidoc.element.mori.isSequential)
- description and source-code
```javascript
function cd(a){return a?a.j&16777216||a.yc?!0:a.j?!1:w(Db,a):w(Db,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isSet"></a>[function <span class="apidocSignatureSpan">mori.</span>isSet (a)](#apidoc.element.mori.isSet)
- description and source-code
```javascript
function ad(a){return null==a?!1:a?a.j&4096||a.zc?!0:a.j?!1:w(jb,a):w(jb,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isSubset"></a>[function <span class="apidocSignatureSpan">mori.</span>isSubset (a, b)](#apidoc.element.mori.isSubset)
- description and source-code
```javascript
isSubset = function (a, b){return Q(a)<=Q(b)&&Ee(function(a){return nd(b,a)},a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isSuperset"></a>[function <span class="apidocSignatureSpan">mori.</span>isSuperset (a, b)](#apidoc.element.mori.isSuperset)
- description and source-code
```javascript
isSuperset = function (a, b){return Q(a)>=Q(b)&&Ee(function(b){return nd(a,b)},b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isSymbol"></a>[function <span class="apidocSignatureSpan">mori.</span>isSymbol (a)](#apidoc.element.mori.isSymbol)
- description and source-code
```javascript
isSymbol = function (a){return a instanceof qc}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.isVector"></a>[function <span class="apidocSignatureSpan">mori.</span>isVector (a)](#apidoc.element.mori.isVector)
- description and source-code
```javascript
function ed(a){return a?a.j&16384||a.Ac?!0:a.j?!1:w(nb,a):w(nb,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.iterate"></a>[function <span class="apidocSignatureSpan">mori.</span>iterate (b, c)](#apidoc.element.mori.iterate)
- description and source-code
```javascript
function Zh(b, c){return M(c,new V(null,function(){return Zh(b,b.b?b.b(c):b.call(null,c))},null,null))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.join"></a>[function <span class="apidocSignatureSpan">mori.</span>join (c, e, f)](#apidoc.element.mori.join)
- description and source-code
```javascript
join = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.juxt"></a>[function <span class="apidocSignatureSpan">mori.</span>juxt (a)](#apidoc.element.mori.juxt)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keep"></a>[function <span class="apidocSignatureSpan">mori.</span>keep (c, e)](#apidoc.element.mori.keep)
- description and source-code
```javascript
keep = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keepIndexed"></a>[function <span class="apidocSignatureSpan">mori.</span>keepIndexed (c, e)](#apidoc.element.mori.keepIndexed)
- description and source-code
```javascript
keepIndexed = function (c, e){switch(arguments.length){case 1:return b.call(this,
c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keys"></a>[function <span class="apidocSignatureSpan">mori.</span>keys (a)](#apidoc.element.mori.keys)
- description and source-code
```javascript
function Tg(a){return(a=D(a))?new Sg(a,null):null}
```
- example usage
```shell
...
'''javascript
var m = mori;
var h = m.hashMap("foo", 1, "bar", 2);

h.has("foo"); // => true
h.get("foo"); // => 1

var iter = h.keys();
iter.next(); // => {done: false, value: "foo"}
'''

This feature is subject to changes in the ES6 proposal.

### Transducers
...
```

#### <a name="apidoc.element.mori.keyword"></a>[function <span class="apidocSignatureSpan">mori.</span>keyword (c, e)](#apidoc.element.mori.keyword)
- description and source-code
```javascript
keyword = function (c, e){switch(arguments.length){case 1:return b.call(this,
c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.knit"></a>[function <span class="apidocSignatureSpan">mori.</span>knit (a)](#apidoc.element.mori.knit)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.last"></a>[function <span class="apidocSignatureSpan">mori.</span>last (a)](#apidoc.element.mori.last)
- description and source-code
```javascript
last = function (a){for(;;){var b=K(a);if(null!=b)a=b;else return G(a)}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lazySeq"></a>[function <span class="apidocSignatureSpan">mori.</span>lazySeq (a)](#apidoc.element.mori.lazySeq)
- description and source-code
```javascript
lazySeq = function (a){return new V(null,a,null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.list"></a>[function <span class="apidocSignatureSpan">mori.</span>list (a)](#apidoc.element.mori.list)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lt"></a>[function <span class="apidocSignatureSpan">mori.</span>lt (a, d, e)](#apidoc.element.mori.lt)
- description and source-code
```javascript
lt = function (a, d, e){switch(arguments.length){case 1:return!0;case 2:return a<d;default:var f=null;if(2<arguments.length){for(var f=
0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lte"></a>[function <span class="apidocSignatureSpan">mori.</span>lte (a, d, e)](#apidoc.element.mori.lte)
- description and source-code
```javascript
lte = function (a, d, e){switch(arguments.length){case 1:return!0;case 2:return a<=d;default:var f=null;if(2<arguments.length){for(var f
=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+
2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map"></a>[function <span class="apidocSignatureSpan">mori.</span>map (e, h, l, m, p)](#apidoc.element.mori.map)
- description and source-code
```javascript
map = function (e, h, l, m, p){switch(arguments.length){case 1:return d.call(this,e);case 2:return c.call(this,e,h);case 3:return b.call(this
,e,h,l);case 4:return a.call(this,
e,h,l,m);default:var q=null;if(4<arguments.length){for(var q=0,s=Array(arguments.length-4);q<s.length;)s[q]=arguments[q+4],++q;q
=new F(s,0)}return f.d(e,h,l,m,q)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
You can use it from your projects like so:

'''javascript
var inc = function(n) {
  return n+1;
};

mori.intoArray(mori.map(inc, mori.vector(1,2,3,4,5)));
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
...
```

#### <a name="apidoc.element.mori.mapIndexed"></a>[function <span class="apidocSignatureSpan">mori.</span>mapIndexed (a, b)](#apidoc.element.mori.mapIndexed)
- description and source-code
```javascript
mapIndexed = function (a, b){return function d(b,f){return new V(null,function(){var g=D(f);if(g){if(fd(g)){for(var h=Yb(g),l=Q(h),m=Td(l),p=0
;;)if(p<l)Xd(m,function(){var d=b+p,f=C.a(h,p);return a.a?a.a(d,f):a.call(null,d,f)}()),p+=1;else break;return Wd(m.ca(),d(b+l,Zb
(g)))}return M(function(){var d=G(g);return a.a?a.a(b,d):a.call(null,b,d)}(),d(b+1,H(g)))}return null},null,null)}(0,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mapInvert"></a>[function <span class="apidocSignatureSpan">mori.</span>mapInvert (a)](#apidoc.element.mori.mapInvert)
- description and source-code
```javascript
function Wh(a){return A.c(function(a,c){var d=R.c(c,0,null),e=R.c(c,1,null);return Rc.c(a,e,d)},Uf,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mapcat"></a>[function <span class="apidocSignatureSpan">mori.</span>mapcat (b, e)](#apidoc.element.mori.mapcat)
- description and source-code
```javascript
mapcat = function (b, e){switch(arguments.length){case 1:return a.call(this,b);default:var f=null;if(1<arguments.length){for(var f=0,g=Array
(arguments.length-1);f<g.length;)g[f]=arguments[f+1],++f;f=new F(g,0)}return c.d(b,f)}throw Error("Invalid arity: "+arguments.length
);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.merge"></a>[function <span class="apidocSignatureSpan">mori.</span>merge (a)](#apidoc.element.mori.merge)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mergeWith"></a>[function <span class="apidocSignatureSpan">mori.</span>mergeWith (a, d)](#apidoc.element.mori.mergeWith)
- description and source-code
```javascript
function a(a, d){var e=null;if(1<arguments.length){for(var e=0,f=Array(arguments.length-1);e<f.length;)f[e]=arguments[e+1],++e;e=
new F(f,0)}return b.call(this,a,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.meta"></a>[function <span class="apidocSignatureSpan">mori.</span>meta (a)](#apidoc.element.mori.meta)
- description and source-code
```javascript
function Vc(a){var b=null!=a;return(b?a?a.j&131072||a.kc||(a.j?0:w(rb,a)):w(rb,a):b)?sb(a):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.assoc"></a>[function <span class="apidocSignatureSpan">mori.</span>mutable.assoc (a, d, e, f)](#apidoc.element.mori.mutable.assoc)
- description and source-code
```javascript
mutable.assoc = function (a, d, e, f){switch(arguments.length){case 3:return Rb(a,d,e);default:var g=null;if(3<arguments.length){for(var g=0,h=Array
(arguments.length-3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return b.d(a,d,e,g)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.conj"></a>[function <span class="apidocSignatureSpan">mori.</span>mutable.conj (b, e, f)](#apidoc.element.mori.mutable.conj)
- description and source-code
```javascript
mutable.conj = function (b, e, f){switch(arguments.length){case 0:return a.call(this);case 1:return b;case 2:return Pb(b,
e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F
(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.disj"></a>[function <span class="apidocSignatureSpan">mori.</span>mutable.disj (a, d, e)](#apidoc.element.mori.mutable.disj)
- description and source-code
```javascript
mutable.disj = function (a, d, e){switch(arguments.length){case 2:return Vb(a,d);default:var f=null;if(2<arguments.length){for(var f=0,g=Array(arguments
.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.dissoc"></a>[function <span class="apidocSignatureSpan">mori.</span>mutable.dissoc (a, d, e)](#apidoc.element.mori.mutable.dissoc)
- description and source-code
```javascript
mutable.dissoc = function (a, d, e){switch(arguments.length){case 2:return Sb(a,d);default:var f=null;if(2<
arguments.length){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw
 Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.next"></a>[function <span class="apidocSignatureSpan">mori.</span>next (a)](#apidoc.element.mori.next)
- description and source-code
```javascript
function K(a){return null==a?null:a&&(a.j&128||a.xb)?a.T(null):D(H(a))}
```
- example usage
```shell
...
var m = mori;
var h = m.hashMap("foo", 1, "bar", 2);

h.has("foo"); // => true
h.get("foo"); // => 1

var iter = h.keys();
iter.next(); // => {done: false, value: "foo"}
'''

This feature is subject to changes in the ES6 proposal.

### Transducers

Mori includes Transducers. Zero allocation collection operations FTW:
...
```

#### <a name="apidoc.element.mori.notEquals"></a>[function <span class="apidocSignatureSpan">mori.</span>notEquals (b, e, f)](#apidoc.element.mori.notEquals)
- description and source-code
```javascript
notEquals = function (b, e, f){switch(arguments.length){case 1:return!1;case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length
){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid
 arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.nth"></a>[function <span class="apidocSignatureSpan">mori.</span>nth (c, e, f)](#apidoc.element.mori.nth)
- description and source-code
```javascript
nth = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial"></a>[function <span class="apidocSignatureSpan">mori.</span>partial (d, g, h, l, m)](#apidoc.element.mori.partial)
- description and source-code
```javascript
partial = function (d, g, h, l, m){switch(arguments.length){case 1:return d;case 2:return c.call(this,d,g);case 3:return b.call(this,d,g,h);case
 4:return a.call(this,d,g,h,l);default:var p=null;if(4<arguments.length){for(var p=
0,q=Array(arguments.length-4);p<q.length;)q[p]=arguments[p+4],++p;p=new F(q,0)}return e.d(d,g,h,l,p)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partition"></a>[function <span class="apidocSignatureSpan">mori.</span>partition (d, f, g, h)](#apidoc.element.mori.partition)
- description and source-code
```javascript
partition = function (d, f, g, h){switch(arguments.length){case 2:return c.call(this,d,f);case 3:return b.call(this,d,f,g);case 4:return a.call
(this,d,f,g,h)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionAll"></a>[function <span class="apidocSignatureSpan">mori.</span>partitionAll (d, f, g)](#apidoc.element.mori.partitionAll)
- description and source-code
```javascript
partitionAll = function (d, f, g){switch(arguments.length){case 1:return c.call(this,d);case 2:return b.call(this,d,f);case 3:return a.call(this,
d,f,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionBy"></a>[function <span class="apidocSignatureSpan">mori.</span>partitionBy (c, e)](#apidoc.element.mori.partitionBy)
- description and source-code
```javascript
partitionBy = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.peek"></a>[function <span class="apidocSignatureSpan">mori.</span>peek (a)](#apidoc.element.mori.peek)
- description and source-code
```javascript
function Wc(a){return null==a?null:lb(a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.pipeline"></a>[function <span class="apidocSignatureSpan">mori.</span>pipeline (a)](#apidoc.element.mori.pipeline)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.pop"></a>[function <span class="apidocSignatureSpan">mori.</span>pop (a)](#apidoc.element.mori.pop)
- description and source-code
```javascript
pop = function (a){return null==a?null:mb(a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.primSeq"></a>[function <span class="apidocSignatureSpan">mori.</span>primSeq (c, e)](#apidoc.element.mori.primSeq)
- description and source-code
```javascript
primSeq = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.project"></a>[function <span class="apidocSignatureSpan">mori.</span>project (a, b)](#apidoc.element.mori.project)
- description and source-code
```javascript
project = function (a, b){return fh(Oe.a(function(a){return Yg(a,b)},a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.queue"></a>[function <span class="apidocSignatureSpan">mori.</span>queue (a)](#apidoc.element.mori.queue)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.range"></a>[function <span class="apidocSignatureSpan">mori.</span>range (e, g, h)](#apidoc.element.mori.range)
- description and source-code
```javascript
range = function (e, g, h){switch(arguments.length){case 0:return d.call(this);case 1:return c.call(this,e);case 2:return b.call(this,e,g);
case 3:return a.call(this,e,g,h)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.reduce"></a>[function <span class="apidocSignatureSpan">mori.</span>reduce (c, e, f)](#apidoc.element.mori.reduce)
- description and source-code
```javascript
reduce = function (c, e, f){switch(arguments.length){case 2:return b.call(this,
c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
v2.toString(); // => '[1 2 3 4]'
'''

'''javascript
var sum = function(a, b) {
  return a + b;
};
mori.reduce(sum, mori.vector(1, 2, 3, 4)); // => 10
'''

Lazy sequences!

'''javascript
var _ = mori;
_.intoArray(_.interpose("foo", _.vector(1, 2, 3, 4)));
...
```

#### <a name="apidoc.element.mori.reduceKV"></a>[function <span class="apidocSignatureSpan">mori.</span>reduceKV (a, b, c)](#apidoc.element.mori.reduceKV)
- description and source-code
```javascript
reduceKV = function (a, b, c){return null!=c?xb(c,a,b):b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.remove"></a>[function <span class="apidocSignatureSpan">mori.</span>remove (c, e)](#apidoc.element.mori.remove)
- description and source-code
```javascript
remove = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.rename"></a>[function <span class="apidocSignatureSpan">mori.</span>rename (a, b)](#apidoc.element.mori.rename)
- description and source-code
```javascript
rename = function (a, b){return fh(Oe.a(function(a){return Uh(a,b)},a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.renameKeys"></a>[function <span class="apidocSignatureSpan">mori.</span>renameKeys (a, b)](#apidoc.element.mori.renameKeys)
- description and source-code
```javascript
function Uh(a, b){return A.c(function(b,d){var e=R.c(d,0,null),f=R.c(d,1,null);return nd(a,e)?Rc.c(b,f,S.a(a,e)):b},T.c(Sc,a,Tg(b
)),b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeat"></a>[function <span class="apidocSignatureSpan">mori.</span>repeat (c, e)](#apidoc.element.mori.repeat)
- description and source-code
```javascript
repeat = function (c, e){switch(arguments.length){case 1:return b.call(this,
c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeatedly"></a>[function <span class="apidocSignatureSpan">mori.</span>repeatedly (c, e)](#apidoc.element.mori.repeatedly)
- description and source-code
```javascript
repeatedly = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.resetMeta"></a>[function <span class="apidocSignatureSpan">mori.</span>resetMeta (a, b)](#apidoc.element.mori.resetMeta)
- description and source-code
```javascript
resetMeta = function (a, b){return a.k=b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.rest"></a>[function <span class="apidocSignatureSpan">mori.</span>rest (a)](#apidoc.element.mori.rest)
- description and source-code
```javascript
function H(a){return null!=a?a&&(a.j&64||a.jb)?a.S(null):(a=D(a))?Wa(a):J:J}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.reverse"></a>[function <span class="apidocSignatureSpan">mori.</span>reverse (a)](#apidoc.element.mori.reverse)
- description and source-code
```javascript
function Jd(a){return Id(a)?Gb(a):A.c(Nc,J,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.second"></a>[function <span class="apidocSignatureSpan">mori.</span>second (a)](#apidoc.element.mori.second)
- description and source-code
```javascript
function Lc(a){return G(K(a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.selectKeys"></a>[function <span class="apidocSignatureSpan">mori.</span>selectKeys (a, b)](#apidoc.element.mori.selectKeys)
- description and source-code
```javascript
function Yg(a, b){for(var c=Uf,d=D(b);;)if(d)var e=G(d),f=S.c(a,e,Zg),c=je.a(f,Zg)?Rc.c(c,e,f):c,d=K(d);else return O(c,Vc(a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.seq"></a>[function <span class="apidocSignatureSpan">mori.</span>seq (a)](#apidoc.element.mori.seq)
- description and source-code
```javascript
function D(a){if(null==a)return null;if(a&&(a.j&8388608||a.mc))return a.D(null);if(a instanceof Array||"string"===typeof a)return
 0===a.length?null:new F(a,0);if(w(Bb,a))return Cb(a);throw Error([z(a),z(" is not ISeqable")].join(""));}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sequence"></a>[function <span class="apidocSignatureSpan">mori.</span>sequence (b, e, f)](#apidoc.element.mori.sequence)
- description and source-code
```javascript
sequence = function (b, e, f){switch(arguments.length){case 1:return a.call(this,b);case 2:return new ze(ye(b,we(e)),null,null,null);default:
var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return
 c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.set"></a>[function <span class="apidocSignatureSpan">mori.</span>set (a)](#apidoc.element.mori.set)
- description and source-code
```javascript
function fh(a){a=D(a);if(null==a)return bh;if(a instanceof F&&0===a.m){a=a.e;a:{for(var b=0,c=Ob(bh);;)if(b<a.length)var d=b+1,c
=c.Sa(null,a[b]),b=d;else{a=c;break a}a=void 0}return a.Ta(null)}for(d=Ob(bh);;)if(null!=a)b=a.T(null),d=d.Sa(null,a.N(null)),a=
b;else return d.Ta(null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.some"></a>[function <span class="apidocSignatureSpan">mori.</span>some (a, b)](#apidoc.element.mori.some)
- description and source-code
```javascript
function Fe(a, b){for(;;)if(D(b)){var c;c=G(b);c=a.b?a.b(c):a.call(null,c);if(t(c))return c;c=a;var d=K(b);a=c;b=d}else return null
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sort"></a>[function <span class="apidocSignatureSpan">mori.</span>sort (c, e)](#apidoc.element.mori.sort)
- description and source-code
```javascript
sort = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortBy"></a>[function <span class="apidocSignatureSpan">mori.</span>sortBy (c, e, f)](#apidoc.element.mori.sortBy)
- description and source-code
```javascript
sortBy = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedMap"></a>[function <span class="apidocSignatureSpan">mori.</span>sortedMap (a)](#apidoc.element.mori.sortedMap)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedMapBy"></a>[function <span class="apidocSignatureSpan">mori.</span>sortedMapBy (a, d)](#apidoc.element.mori.sortedMapBy)
- description and source-code
```javascript
function a(a, d){var e=null;if(1<arguments.length){for(var e=0,f=Array(arguments.length-1);e<f.length;)f[e]=arguments[e+1],++e;e=
new F(f,0)}return b.call(this,a,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedSet"></a>[function <span class="apidocSignatureSpan">mori.</span>sortedSet (a)](#apidoc.element.mori.sortedSet)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedSetBy"></a>[function <span class="apidocSignatureSpan">mori.</span>sortedSetBy (a, d)](#apidoc.element.mori.sortedSetBy)
- description and source-code
```javascript
function a(a, d){var e=null;if(1<arguments.length){for(var e=0,f=Array(arguments.length-1);e<f.length;)f[e]=arguments[e+1],++e;e=
new F(f,0)}return b.call(this,a,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subseq"></a>[function <span class="apidocSignatureSpan">mori.</span>subseq (c, e, f, g, h)](#apidoc.element.mori.subseq)
- description and source-code
```javascript
subseq = function (c, e, f, g, h){switch(arguments.length){case 3:return b.call(this,c,e,f);case 5:return a.call(this,c,e,f,g,h)}throw Error("
Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subvec"></a>[function <span class="apidocSignatureSpan">mori.</span>subvec (c, e, f)](#apidoc.element.mori.subvec)
- description and source-code
```javascript
subvec = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sum"></a>[function <span class="apidocSignatureSpan">mori.</span>sum (a, d, e)](#apidoc.element.mori.sum)
- description and source-code
```javascript
sum = function (a, d, e){switch(arguments.length){case 0:return 0;case 1:return a;case 2:return a+d;default:var f=null;if(2<arguments.length
){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,
0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.symbol"></a>[function <span class="apidocSignatureSpan">mori.</span>symbol (c, e)](#apidoc.element.mori.symbol)
- description and source-code
```javascript
symbol = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.take"></a>[function <span class="apidocSignatureSpan">mori.</span>take (c, e)](#apidoc.element.mori.take)
- description and source-code
```javascript
take = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,
c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeNth"></a>[function <span class="apidocSignatureSpan">mori.</span>takeNth (c, e)](#apidoc.element.mori.takeNth)
- description and source-code
```javascript
takeNth = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeWhile"></a>[function <span class="apidocSignatureSpan">mori.</span>takeWhile (c, e)](#apidoc.element.mori.takeWhile)
- description and source-code
```javascript
takeWhile = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.toClj"></a>[function <span class="apidocSignatureSpan">mori.</span>toClj (c, e)](#apidoc.element.mori.toClj)
- description and source-code
```javascript
toClj = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.toJs"></a>[function <span class="apidocSignatureSpan">mori.</span>toJs (b)](#apidoc.element.mori.toJs)
- description and source-code
```javascript
function Lh(b){if(null==b)return null;if(b?t(t(null)?null:b.fc)||(b.yb?0:w(Hh,b)):w(Hh,b))return Ih(b);if(b instanceof U)return
Od(b);if(b instanceof qc)return""+z(b);if(dd(b)){var c={};b=D(b);for(var d=null,e=0,f=0;;)if(f<e){var g=d.Q(null,f),h=R.c(g,0,null
),g=R.c(g,1,null);c[Jh(h)]=Lh(g);f+=1}else if(b=D(b))fd(b)?(e=Yb(b),b=Zb(b),d=e,e=Q(e)):(e=G(b),d=R.c(e,0,null),e=R.c(e,1,null),
c[Jh(d)]=Lh(e),b=K(b),d=null,e=0),f=0;else break;return c}if($c(b)){c=[];b=D(Oe.a(Lh,b));d=null;for(f=e=0;;)if(f<
e)h=d.Q(null,f),c.push(h),f+=1;else if(b=D(b))d=b,fd(d)?(b=Yb(d),f=Zb(d),d=b,e=Q(b),b=f):(b=G(d),c.push(b),b=K(d),d=null,e=0),f=
0;else break;return c}return b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.transduce"></a>[function <span class="apidocSignatureSpan">mori.</span>transduce (c, e, f, g)](#apidoc.element.mori.transduce)
- description and source-code
```javascript
transduce = function (c, e, f, g){switch(arguments.length){case 3:return b.call(this,c,e,f);case 4:return a.call(this,c,e,f,g)}throw Error("Invalid
 arity: "+arguments.length);}
```
- example usage
```shell
...
  f();
  console.log(((new Date())-s)+"ms");
}

// ~190ms V8 version 3.29.80 MBP 2.26ghz
time(function() {
  var xf = m.comp(m.map(m.inc), m.map(m.inc), m.map(m.inc));
  return m.transduce(xf, m.completing(m.sum), 0, v);
}, 10);

// ~440ms
time(function() {
  return a.map(m.inc).map(m.inc).map(m.inc).reduce(function(a,b){return a+b;}, 0);
}, 10);
'''
...
```

#### <a name="apidoc.element.mori.union"></a>[function <span class="apidocSignatureSpan">mori.</span>union (b, e, f)](#apidoc.element.mori.union)
- description and source-code
```javascript
union = function (b, e, f){switch(arguments.length){case 0:return bh;case 1:return b;
case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g
]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn"></a>[function <span class="apidocSignatureSpan">mori.</span>updateIn (e, h, l, m, p, q, s)](#apidoc.element.mori.updateIn)
- description and source-code
```javascript
updateIn = function (e, h, l, m, p, q, s){switch(arguments.length){case 3:return d.call(this,e,h,l);case 4:return c.call(this,e,h,l,m);case 5:return
 b.call(this,e,h,l,m,p);case 6:return a.call(this,e,h,l,m,p,q);default:var u=null;if(6<arguments.length){for(var u=0,v=Array(arguments
.length-6);u<v.length;)v[u]=arguments[u+6],++u;u=new F(v,0)}return f.d(e,h,l,m,p,q,u)}throw Error("Invalid arity: "+arguments.length
);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.vals"></a>[function <span class="apidocSignatureSpan">mori.</span>vals (a)](#apidoc.element.mori.vals)
- description and source-code
```javascript
function Vg(a){return(a=D(a))?new Ug(a,null):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta"></a>[function <span class="apidocSignatureSpan">mori.</span>varyMeta (f, l, m, p, q, s, u)](#apidoc.element.mori.varyMeta)
- description and source-code
```javascript
varyMeta = function (f, l, m, p, q, s, u){switch(arguments.length){case 2:return e.call(this,f,l);case 3:return d.call(this,f,l,m);case 4:return
c.call(this,f,l,m,p);case 5:return b.call(this,f,l,m,p,q);case 6:return a.call(this,f,l,m,p,q,s);default:var v=null;if(6<arguments
.length){for(var v=
0,y=Array(arguments.length-6);v<y.length;)y[v]=arguments[v+6],++v;v=new F(y,0)}return g.d(f,l,m,p,q,s,v)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.vector"></a>[function <span class="apidocSignatureSpan">mori.</span>vector (a)](#apidoc.element.mori.vector)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
...
You can use it from your projects like so:

'''javascript
var inc = function(n) {
  return n+1;
};

mori.intoArray(mori.map(inc, mori.vector(1,2,3,4,5)));
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
...
```

#### <a name="apidoc.element.mori.withMeta"></a>[function <span class="apidocSignatureSpan">mori.</span>withMeta (a, b)](#apidoc.element.mori.withMeta)
- description and source-code
```javascript
function O(a, b){return Tc(a)&&!(a?a.j&262144||a.Bc||(a.j?0:w(tb,a)):w(tb,a))?new Uc(a,b):null==a?null:ub(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.zipmap"></a>[function <span class="apidocSignatureSpan">mori.</span>zipmap (a, b)](#apidoc.element.mori.zipmap)
- description and source-code
```javascript
zipmap = function (a, b){for(var c=Ob(Uf),d=D(a),e=D(b);;)if(d&&e)c=ee.c(c,G(d),G(e)),d=K(d),e=K(e);else return Qb(c)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.alterMeta"></a>[module mori.alterMeta](#apidoc.module.mori.alterMeta)

#### <a name="apidoc.element.mori.alterMeta.alterMeta"></a>[function <span class="apidocSignatureSpan">mori.</span>alterMeta (a, d, e)](#apidoc.element.mori.alterMeta.alterMeta)
- description and source-code
```javascript
function a(a, d, e){var f=null;if(2<arguments.length){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;
f=new F(g,0)}return b.call(this,a,d,f)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.alterMeta.d"></a>[function <span class="apidocSignatureSpan">mori.alterMeta.</span>d (a, b, e)](#apidoc.element.mori.alterMeta.d)
- description and source-code
```javascript
function b(a, b, e){return a.k=T.c(b,a.k,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.alterMeta.f"></a>[function <span class="apidocSignatureSpan">mori.alterMeta.</span>f (a)](#apidoc.element.mori.alterMeta.f)
- description and source-code
```javascript
f = function (a){var d=G(a);a=K(a);var e=G(a);a=H(a);return b(d,e,a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.apply"></a>[module mori.apply](#apidoc.module.mori.apply)

#### <a name="apidoc.element.mori.apply.apply"></a>[function <span class="apidocSignatureSpan">mori.</span>apply ()](#apidoc.element.mori.apply.apply)
- description and source-code
```javascript
function apply() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.a"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>a (a, b)](#apidoc.element.mori.apply.a)
- description and source-code
```javascript
function d(a, b){var c=a.i;if(a.f){var d=Yd(b,c+1);return d<=c?he(a,d,b):a.f(b)}return a.apply(a,rd(b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.c"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>c (a, b, c)](#apidoc.element.mori.apply.c)
- description and source-code
```javascript
function c(a, b, c){b=be.a(b,c);c=a.i;if(a.f){var d=Yd(b,c+1);return d<=c?he(a,d,b):a.f(b)}return a.apply(a,rd(b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.d"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>d (a, c, d, e, f, g)](#apidoc.element.mori.apply.d)
- description and source-code
```javascript
function b(a, c, d, e, f, g){c=M(c,M(d,M(e,M(f,$d(g)))));d=a.i;return a.f?(e=Yd(c,d+1),e<=d?he(a,e,c):a.f(c)):a.apply(a,rd(c))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.f"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>f (a)](#apidoc.element.mori.apply.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=K(a);var e=G(a);a=K(a);var f=G(a);a=K(a);var g=G(a);a=H(a);return b(c,d,e,f,g,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.f2"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>f2 (a, b)](#apidoc.element.mori.apply.f2)
- description and source-code
```javascript
function d(a, b){var c=a.i;if(a.f){var d=Yd(b,c+1);return d<=c?he(a,d,b):a.f(b)}return a.apply(a,rd(b))}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.apply.f3"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>f3 (a, b, c)](#apidoc.element.mori.apply.f3)
- description and source-code
```javascript
function c(a, b, c){b=be.a(b,c);c=a.i;if(a.f){var d=Yd(b,c+1);return d<=c?he(a,d,b):a.f(b)}return a.apply(a,rd(b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.f4"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>f4 (a, b, c, d)](#apidoc.element.mori.apply.f4)
- description and source-code
```javascript
function b(a, b, c, d){b=be.c(b,c,d);c=a.i;return a.f?(d=Yd(b,c+1),d<=c?he(a,d,b):a.f(b)):a.apply(a,rd(b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.f5"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>f5 (a, b, c, d, e)](#apidoc.element.mori.apply.f5)
- description and source-code
```javascript
function a(a, b, c, d, e){b=be.n(b,c,d,e);c=a.i;return a.f?(d=Yd(b,c+1),d<=c?he(a,d,b):a.f(b)):a.apply(a,rd(b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.n"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>n (a, b, c, d)](#apidoc.element.mori.apply.n)
- description and source-code
```javascript
function b(a, b, c, d){b=be.c(b,c,d);c=a.i;return a.f?(d=Yd(b,c+1),d<=c?he(a,d,b):a.f(b)):a.apply(a,rd(b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.apply.r"></a>[function <span class="apidocSignatureSpan">mori.apply.</span>r (a, b, c, d, e)](#apidoc.element.mori.apply.r)
- description and source-code
```javascript
function a(a, b, c, d, e){b=be.n(b,c,d,e);c=a.i;return a.f?(d=Yd(b,c+1),d<=c?he(a,d,b):a.f(b)):a.apply(a,rd(b))}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.assoc"></a>[module mori.assoc](#apidoc.module.mori.assoc)

#### <a name="apidoc.element.mori.assoc.assoc"></a>[function <span class="apidocSignatureSpan">mori.</span>assoc (b, e, f, g)](#apidoc.element.mori.assoc.assoc)
- description and source-code
```javascript
assoc = function (b, e, f, g){switch(arguments.length){case 3:return a.call(this,b,e,f);default:var h=null;if(3<arguments.length){for(var h
=0,l=Array(arguments.length-3);h<l.length;)l[h]=arguments[h+3],++h;h=new F(l,0)}return c.d(b,e,f,h)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.assoc.c"></a>[function <span class="apidocSignatureSpan">mori.assoc.</span>c (a, b, c)](#apidoc.element.mori.assoc.c)
- description and source-code
```javascript
function a(a, b, c){if(null!=a)a=cb(a,b,c);else a:{a=[b];c=[c];b=a.length;for(var g=0,h=Ob(Qc);;)if(g<b)var l=g+1,h=h.kb(null,a[g],
c[g]),g=l;else{a=Qb(h);break a}a=void 0}return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.assoc.d"></a>[function <span class="apidocSignatureSpan">mori.assoc.</span>d (a, d, e, l)](#apidoc.element.mori.assoc.d)
- description and source-code
```javascript
function c(a, d, e, l){for(;;)if(a=b.c(a,
d,e),t(l))d=G(l),e=Lc(l),l=K(K(l));else return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.assoc.f"></a>[function <span class="apidocSignatureSpan">mori.assoc.</span>f (a)](#apidoc.element.mori.assoc.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var d=G(a);a=K(a);var l=G(a);a=H(a);return c(b,d,l,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.assoc.f3"></a>[function <span class="apidocSignatureSpan">mori.assoc.</span>f3 (a, b, c)](#apidoc.element.mori.assoc.f3)
- description and source-code
```javascript
function a(a, b, c){if(null!=a)a=cb(a,b,c);else a:{a=[b];c=[c];b=a.length;for(var g=0,h=Ob(Qc);;)if(g<b)var l=g+1,h=h.kb(null,a[g],
c[g]),g=l;else{a=Qb(h);break a}a=void 0}return a}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.comp"></a>[module mori.comp](#apidoc.module.mori.comp)

#### <a name="apidoc.element.mori.comp.comp"></a>[function <span class="apidocSignatureSpan">mori.</span>comp (c, f, g, h)](#apidoc.element.mori.comp.comp)
- description and source-code
```javascript
comp = function (c, f, g, h){switch(arguments.length){case 0:return ud;case 1:return c;case 2:return b.call(this,c,f);case 3:return a.call
(this,c,f,g);default:var l=null;if(3<arguments.length){for(var l=0,m=Array(arguments.length-3);l<m.length;)m[l]=arguments[l+3],++
l;l=new F(m,0)}return d.d(c,f,g,l)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
  var s = new Date();
  f();
  console.log(((new Date())-s)+"ms");
}

// ~190ms V8 version 3.29.80 MBP 2.26ghz
time(function() {
  var xf = m.comp(m.map(m.inc), m.map(m.inc), m.map(m.inc));
  return m.transduce(xf, m.completing(m.sum), 0, v);
}, 10);

// ~440ms
time(function() {
  return a.map(m.inc).map(m.inc).map(m.inc).reduce(function(a,b){return a+b;}, 0);
}, 10);
...
```

#### <a name="apidoc.element.mori.comp.a"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>a (a, b)](#apidoc.element.mori.comp.a)
- description and source-code
```javascript
function b(a, b){return function(){function c(d,g,h){d=b.c?b.c(d,g,h):b.call(null,d,g,h);return a.b?a.b(d):a.call(null,d)}function
 d(c,g){var h=b.a?b.a(c,g):b.call(null,c,g);return a.b?a.b(h):a.call(null,h)}
function l(c){c=b.b?b.b(c):b.call(null,c);return a.b?a.b(c):a.call(null,c)}function m(){var c=b.l?b.l():b.call(null);return a.b?
a.b(c):a.call(null,c)}var p=null,q=function(){function c(a,b,e,f){var g=null;if(3<arguments.length){for(var g=0,h=Array(arguments
.length-3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return d.call(this,a,b,e,g)}function d(c,g,h,l){c=T.r(b,c,g,h,l);return
 a.b?a.b(c):a.call(null,c)}c.i=3;c.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var e=G(a);a=H(a);return d(b,
c,e,a)};c.d=d;return c}(),p=function(a,b,e,f){switch(arguments.length){case 0:return m.call(this);case 1:return l.call(this,a);case
 2:return d.call(this,a,b);case 3:return c.call(this,a,b,e);default:var p=null;if(3<arguments.length){for(var p=0,E=Array(arguments
.length-3);p<E.length;)E[p]=arguments[p+3],++p;p=new F(E,0)}return q.d(a,b,e,p)}throw Error("Invalid arity: "+arguments.length);};
p.i=3;p.f=q.f;p.l=m;p.b=l;p.a=d;p.c=c;p.d=q.d;return p}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp.b"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>b (a)](#apidoc.element.mori.comp.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp.c"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>c (a, b, c)](#apidoc.element.mori.comp.c)
- description and source-code
```javascript
function a(a, b, c){return function(){function d(h,l,m){h=c.c?c.c(h,l,m):c.call(null,h,l,m);h=b.b?b.b(h):b.call(null,h);return a.b
?a.b(h):a.call(null,h)}function l(d,h){var l;l=c.a?c.a(d,h):c.call(null,d,h);l=b.b?b.b(l):b.call(null,l);return a.b?a.b(l):a.call
(null,l)}function m(d){d=c.b?c.b(d):c.call(null,d);d=b.b?b.b(d):b.call(null,d);return a.b?a.b(d):a.call(null,d)}function p(){var
 d;d=c.l?c.l():c.call(null);d=b.b?b.b(d):b.call(null,d);return a.b?a.b(d):a.call(null,d)}var q=null,
s=function(){function d(a,b,c,e){var f=null;if(3<arguments.length){for(var f=0,g=Array(arguments.length-3);f<g.length;)g[f]=arguments
[f+3],++f;f=new F(g,0)}return h.call(this,a,b,c,f)}function h(d,l,m,p){d=T.r(c,d,l,m,p);d=b.b?b.b(d):b.call(null,d);return a.b?a
.b(d):a.call(null,d)}d.i=3;d.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return h(b,c,d,a)};d.d=h;return
 d}(),q=function(a,b,c,e){switch(arguments.length){case 0:return p.call(this);case 1:return m.call(this,a);case 2:return l.call(
this,
a,b);case 3:return d.call(this,a,b,c);default:var f=null;if(3<arguments.length){for(var f=0,g=Array(arguments.length-3);f<g.length
;)g[f]=arguments[f+3],++f;f=new F(g,0)}return s.d(a,b,c,f)}throw Error("Invalid arity: "+arguments.length);};q.i=3;q.f=s.f;q.l=p
;q.b=m;q.a=l;q.c=d;q.d=s.d;return q}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp.d"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>d (a, c, d, e)](#apidoc.element.mori.comp.d)
- description and source-code
```javascript
function b(a, c, d, e){return function(a){return function(){function b(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments
.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new F(e,0)}return c.call(this,d)}function c(b){b=T.a(G(a),b);for(var d=K(a);;)if
(d)b=G(d).call(null,b),d=K(d);else return b}b.i=0;b.f=function(a){a=D(a);return c(a)};b.d=c;return b}()}(Jd(be.n(a,
c,d,e)))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp.f"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>f (a)](#apidoc.element.mori.comp.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=K(a);var e=G(a);a=H(a);return b(c,d,e,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp.f0"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>f0 ()](#apidoc.element.mori.comp.f0)
- description and source-code
```javascript
f0 = function (){return ud}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp.f1"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>f1 (a)](#apidoc.element.mori.comp.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp.f2"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>f2 (a, b)](#apidoc.element.mori.comp.f2)
- description and source-code
```javascript
function b(a, b){return function(){function c(d,g,h){d=b.c?b.c(d,g,h):b.call(null,d,g,h);return a.b?a.b(d):a.call(null,d)}function
 d(c,g){var h=b.a?b.a(c,g):b.call(null,c,g);return a.b?a.b(h):a.call(null,h)}
function l(c){c=b.b?b.b(c):b.call(null,c);return a.b?a.b(c):a.call(null,c)}function m(){var c=b.l?b.l():b.call(null);return a.b?
a.b(c):a.call(null,c)}var p=null,q=function(){function c(a,b,e,f){var g=null;if(3<arguments.length){for(var g=0,h=Array(arguments
.length-3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return d.call(this,a,b,e,g)}function d(c,g,h,l){c=T.r(b,c,g,h,l);return
 a.b?a.b(c):a.call(null,c)}c.i=3;c.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var e=G(a);a=H(a);return d(b,
c,e,a)};c.d=d;return c}(),p=function(a,b,e,f){switch(arguments.length){case 0:return m.call(this);case 1:return l.call(this,a);case
 2:return d.call(this,a,b);case 3:return c.call(this,a,b,e);default:var p=null;if(3<arguments.length){for(var p=0,E=Array(arguments
.length-3);p<E.length;)E[p]=arguments[p+3],++p;p=new F(E,0)}return q.d(a,b,e,p)}throw Error("Invalid arity: "+arguments.length);};
p.i=3;p.f=q.f;p.l=m;p.b=l;p.a=d;p.c=c;p.d=q.d;return p}()}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.comp.f3"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>f3 (a, b, c)](#apidoc.element.mori.comp.f3)
- description and source-code
```javascript
function a(a, b, c){return function(){function d(h,l,m){h=c.c?c.c(h,l,m):c.call(null,h,l,m);h=b.b?b.b(h):b.call(null,h);return a.b
?a.b(h):a.call(null,h)}function l(d,h){var l;l=c.a?c.a(d,h):c.call(null,d,h);l=b.b?b.b(l):b.call(null,l);return a.b?a.b(l):a.call
(null,l)}function m(d){d=c.b?c.b(d):c.call(null,d);d=b.b?b.b(d):b.call(null,d);return a.b?a.b(d):a.call(null,d)}function p(){var
 d;d=c.l?c.l():c.call(null);d=b.b?b.b(d):b.call(null,d);return a.b?a.b(d):a.call(null,d)}var q=null,
s=function(){function d(a,b,c,e){var f=null;if(3<arguments.length){for(var f=0,g=Array(arguments.length-3);f<g.length;)g[f]=arguments
[f+3],++f;f=new F(g,0)}return h.call(this,a,b,c,f)}function h(d,l,m,p){d=T.r(c,d,l,m,p);d=b.b?b.b(d):b.call(null,d);return a.b?a
.b(d):a.call(null,d)}d.i=3;d.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return h(b,c,d,a)};d.d=h;return
 d}(),q=function(a,b,c,e){switch(arguments.length){case 0:return p.call(this);case 1:return m.call(this,a);case 2:return l.call(
this,
a,b);case 3:return d.call(this,a,b,c);default:var f=null;if(3<arguments.length){for(var f=0,g=Array(arguments.length-3);f<g.length
;)g[f]=arguments[f+3],++f;f=new F(g,0)}return s.d(a,b,c,f)}throw Error("Invalid arity: "+arguments.length);};q.i=3;q.f=s.f;q.l=p
;q.b=m;q.a=l;q.c=d;q.d=s.d;return q}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.comp.l"></a>[function <span class="apidocSignatureSpan">mori.comp.</span>l ()](#apidoc.element.mori.comp.l)
- description and source-code
```javascript
l = function (){return ud}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.completing"></a>[module mori.completing](#apidoc.module.mori.completing)

#### <a name="apidoc.element.mori.completing.completing"></a>[function <span class="apidocSignatureSpan">mori.</span>completing (c, e)](#apidoc.element.mori.completing.completing)
- description and source-code
```javascript
completing = function (c, e){switch(arguments.length){case 1:return b.call(this,
c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
  f();
  console.log(((new Date())-s)+"ms");
}

// ~190ms V8 version 3.29.80 MBP 2.26ghz
time(function() {
  var xf = m.comp(m.map(m.inc), m.map(m.inc), m.map(m.inc));
  return m.transduce(xf, m.completing(m.sum), 0, v);
}, 10);

// ~440ms
time(function() {
  return a.map(m.inc).map(m.inc).map(m.inc).reduce(function(a,b){return a+b;}, 0);
}, 10);
'''
...
```

#### <a name="apidoc.element.mori.completing.a"></a>[function <span class="apidocSignatureSpan">mori.completing.</span>a (a, b)](#apidoc.element.mori.completing.a)
- description and source-code
```javascript
function a(a, b){return function(){function c(b,e){return a.a?a.a(b,e):a.call(null,b,e)}function g(a){return b.b?b.b(a):b.call(null
,a)}function h(){return a.l?a.l():a.call(null)}var l=null,l=function(a,b){switch(arguments.length){case 0:return h.call(this);case
 1:return g.call(this,a);case 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};l.l=h;l.b=g;l.a=c;return
 l}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.completing.b"></a>[function <span class="apidocSignatureSpan">mori.completing.</span>b (a)](#apidoc.element.mori.completing.b)
- description and source-code
```javascript
function b(a){return c.a(a,ud)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.completing.f1"></a>[function <span class="apidocSignatureSpan">mori.completing.</span>f1 (a)](#apidoc.element.mori.completing.f1)
- description and source-code
```javascript
function b(a){return c.a(a,ud)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.completing.f2"></a>[function <span class="apidocSignatureSpan">mori.completing.</span>f2 (a, b)](#apidoc.element.mori.completing.f2)
- description and source-code
```javascript
function a(a, b){return function(){function c(b,e){return a.a?a.a(b,e):a.call(null,b,e)}function g(a){return b.b?b.b(a):b.call(null
,a)}function h(){return a.l?a.l():a.call(null)}var l=null,l=function(a,b){switch(arguments.length){case 0:return h.call(this);case
 1:return g.call(this,a);case 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};l.l=h;l.b=g;l.a=c;return
 l}()}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.concat"></a>[module mori.concat](#apidoc.module.mori.concat)

#### <a name="apidoc.element.mori.concat.concat"></a>[function <span class="apidocSignatureSpan">mori.</span>concat (d, g, h)](#apidoc.element.mori.concat.concat)
- description and source-code
```javascript
concat = function (d, g, h){switch(arguments.length){case 0:return c.call(this);case 1:return b.call(this,d);case 2:return a.call(this,d,g);
default:var l=null;if(2<arguments.length){for(var l=0,m=
Array(arguments.length-2);l<m.length;)m[l]=arguments[l+2],++l;l=new F(m,0)}return e.d(d,g,l)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.concat.a"></a>[function <span class="apidocSignatureSpan">mori.concat.</span>a (a, b)](#apidoc.element.mori.concat.a)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var c=D(a);return c?fd(c)?Wd(Yb(c),d.a(Zb(c),b)):M(G(c),d.a(H(c),b)):b},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.concat.b"></a>[function <span class="apidocSignatureSpan">mori.concat.</span>b (a)](#apidoc.element.mori.concat.b)
- description and source-code
```javascript
function b(a){return new V(null,function(){return a},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.concat.d"></a>[function <span class="apidocSignatureSpan">mori.concat.</span>d (a, c, e)](#apidoc.element.mori.concat.d)
- description and source-code
```javascript
function b(a, c, e){return function q(a,b){return new V(null,function(){var c=D(a);return c?fd(c)?Wd(Yb(c),q(Zb(c),b)):M(G(c),q(H(
c),b)):t(b)?q(G(b),K(b)):null},null,null)}(d.a(a,c),e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.concat.f"></a>[function <span class="apidocSignatureSpan">mori.concat.</span>f (a)](#apidoc.element.mori.concat.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=H(a);return b(c,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.concat.f0"></a>[function <span class="apidocSignatureSpan">mori.concat.</span>f0 ()](#apidoc.element.mori.concat.f0)
- description and source-code
```javascript
function c(){return new V(null,function(){return null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.concat.f1"></a>[function <span class="apidocSignatureSpan">mori.concat.</span>f1 (a)](#apidoc.element.mori.concat.f1)
- description and source-code
```javascript
function b(a){return new V(null,function(){return a},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.concat.f2"></a>[function <span class="apidocSignatureSpan">mori.concat.</span>f2 (a, b)](#apidoc.element.mori.concat.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var c=D(a);return c?fd(c)?Wd(Yb(c),d.a(Zb(c),b)):M(G(c),d.a(H(c),b)):b},null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.concat.l"></a>[function <span class="apidocSignatureSpan">mori.concat.</span>l ()](#apidoc.element.mori.concat.l)
- description and source-code
```javascript
function c(){return new V(null,function(){return null},null,null)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.conj"></a>[module mori.conj](#apidoc.module.mori.conj)

#### <a name="apidoc.element.mori.conj.conj"></a>[function <span class="apidocSignatureSpan">mori.</span>conj (b, e, f)](#apidoc.element.mori.conj.conj)
- description and source-code
```javascript
conj = function (b, e, f){switch(arguments.length){case 0:return Mc;case 1:return b;
case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g
]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
var v2 = mori.conj(v1, 4);
v1.toString(); // => '[1 2 3]'
v2.toString(); // => '[1 2 3 4]'
'''

'''javascript
var sum = function(a, b) {
return a + b;
...
```

#### <a name="apidoc.element.mori.conj.a"></a>[function <span class="apidocSignatureSpan">mori.conj.</span>a (a, b)](#apidoc.element.mori.conj.a)
- description and source-code
```javascript
function a(a, b){return null!=a?Ra(a,b):Ra(J,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.conj.b"></a>[function <span class="apidocSignatureSpan">mori.conj.</span>b (a)](#apidoc.element.mori.conj.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.conj.d"></a>[function <span class="apidocSignatureSpan">mori.conj.</span>d (a, d, e)](#apidoc.element.mori.conj.d)
- description and source-code
```javascript
function c(a, d, e){for(;;)if(t(e))a=b.a(a,d),d=G(e),e=K(e);else return b.a(a,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.conj.f"></a>[function <span class="apidocSignatureSpan">mori.conj.</span>f (a)](#apidoc.element.mori.conj.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var d=G(a);a=H(a);return c(b,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.conj.f0"></a>[function <span class="apidocSignatureSpan">mori.conj.</span>f0 ()](#apidoc.element.mori.conj.f0)
- description and source-code
```javascript
f0 = function (){return Mc}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.conj.f1"></a>[function <span class="apidocSignatureSpan">mori.conj.</span>f1 (a)](#apidoc.element.mori.conj.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.conj.f2"></a>[function <span class="apidocSignatureSpan">mori.conj.</span>f2 (a, b)](#apidoc.element.mori.conj.f2)
- description and source-code
```javascript
function a(a, b){return null!=a?Ra(a,b):Ra(J,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.conj.l"></a>[function <span class="apidocSignatureSpan">mori.conj.</span>l ()](#apidoc.element.mori.conj.l)
- description and source-code
```javascript
l = function (){return Mc}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.curry"></a>[module mori.curry](#apidoc.module.mori.curry)

#### <a name="apidoc.element.mori.curry.curry"></a>[function <span class="apidocSignatureSpan">mori.</span>curry (a, d)](#apidoc.element.mori.curry.curry)
- description and source-code
```javascript
function a(a, d){var e=null;if(1<arguments.length){for(var e=0,f=Array(arguments.length-1);e<f.length;)f[e]=arguments[e+1],++e;e=
new F(f,0)}return b.call(this,a,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.curry.d"></a>[function <span class="apidocSignatureSpan">mori.curry.</span>d (a, b)](#apidoc.element.mori.curry.d)
- description and source-code
```javascript
function b(a, b){return function(e){return T.a(a,M.a?M.a(e,b):M.call(null,e,b))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.curry.f"></a>[function <span class="apidocSignatureSpan">mori.curry.</span>f (a)](#apidoc.element.mori.curry.f)
- description and source-code
```javascript
f = function (a){var d=G(a);a=H(a);return b(d,a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.dedupe"></a>[module mori.dedupe](#apidoc.module.mori.dedupe)

#### <a name="apidoc.element.mori.dedupe.dedupe"></a>[function <span class="apidocSignatureSpan">mori.</span>dedupe (c)](#apidoc.element.mori.dedupe.dedupe)
- description and source-code
```javascript
dedupe = function (c){switch(arguments.length){case 0:return b.call(this);case 1:return a.call(this,c)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dedupe.b"></a>[function <span class="apidocSignatureSpan">mori.dedupe.</span>b (a)](#apidoc.element.mori.dedupe.b)
- description and source-code
```javascript
function a(a){return Ce.a(c.l(),a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dedupe.f0"></a>[function <span class="apidocSignatureSpan">mori.dedupe.</span>f0 ()](#apidoc.element.mori.dedupe.f0)
- description and source-code
```javascript
function b(){return function(a){return function(b){return function(){function c(f,g){var h=L.b?L.b(b):L.call(null,b);ac(b,g);return
 sc.a(h,g)?f:a.a?a.a(f,g):a.call(null,f,g)}function g(b){return a.b?a.b(b):a.call(null,b)}function h(){return a.l?a.l():a.call(null
)}var l=null,l=function(a,b){switch(arguments.length){case 0:return h.call(this);case 1:return g.call(this,a);case 2:return c.call
(this,a,b)}throw Error("Invalid arity: "+arguments.length);
};l.l=h;l.b=g;l.a=c;return l}()}(new Me(sh))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dedupe.f1"></a>[function <span class="apidocSignatureSpan">mori.dedupe.</span>f1 (a)](#apidoc.element.mori.dedupe.f1)
- description and source-code
```javascript
function a(a){return Ce.a(c.l(),a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dedupe.l"></a>[function <span class="apidocSignatureSpan">mori.dedupe.</span>l ()](#apidoc.element.mori.dedupe.l)
- description and source-code
```javascript
function b(){return function(a){return function(b){return function(){function c(f,g){var h=L.b?L.b(b):L.call(null,b);ac(b,g);return
 sc.a(h,g)?f:a.a?a.a(f,g):a.call(null,f,g)}function g(b){return a.b?a.b(b):a.call(null,b)}function h(){return a.l?a.l():a.call(null
)}var l=null,l=function(a,b){switch(arguments.length){case 0:return h.call(this);case 1:return g.call(this,a);case 2:return c.call
(this,a,b)}throw Error("Invalid arity: "+arguments.length);
};l.l=h;l.b=g;l.a=c;return l}()}(new Me(sh))}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.difference"></a>[module mori.difference](#apidoc.module.mori.difference)

#### <a name="apidoc.element.mori.difference.difference"></a>[function <span class="apidocSignatureSpan">mori.</span>difference (b, e, f)](#apidoc.element.mori.difference.difference)
- description and source-code
```javascript
difference = function (b, e, f){switch(arguments.length){case 1:return b;case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length
){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid
 arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.difference.a"></a>[function <span class="apidocSignatureSpan">mori.difference.</span>a (a, b)](#apidoc.element.mori.difference.a)
- description and source-code
```javascript
function a(a, b){return Q(a)<Q(b)?A.c(function(a,c){return nd(b,c)?Xc.a(a,c):a},a,a):A.c(Xc,a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.difference.b"></a>[function <span class="apidocSignatureSpan">mori.difference.</span>b (a)](#apidoc.element.mori.difference.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.difference.d"></a>[function <span class="apidocSignatureSpan">mori.difference.</span>d (a, d, e)](#apidoc.element.mori.difference.d)
- description and source-code
```javascript
function c(a, d, e){return A.c(b,a,Nc.a(e,d))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.difference.f"></a>[function <span class="apidocSignatureSpan">mori.difference.</span>f (a)](#apidoc.element.mori.difference.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var d=G(a);a=H(a);return c(b,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.difference.f1"></a>[function <span class="apidocSignatureSpan">mori.difference.</span>f1 (a)](#apidoc.element.mori.difference.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.difference.f2"></a>[function <span class="apidocSignatureSpan">mori.difference.</span>f2 (a, b)](#apidoc.element.mori.difference.f2)
- description and source-code
```javascript
function a(a, b){return Q(a)<Q(b)?A.c(function(a,c){return nd(b,c)?Xc.a(a,c):a},a,a):A.c(Xc,a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.disj"></a>[module mori.disj](#apidoc.module.mori.disj)

#### <a name="apidoc.element.mori.disj.disj"></a>[function <span class="apidocSignatureSpan">mori.</span>disj (b, e, f)](#apidoc.element.mori.disj.disj)
- description and source-code
```javascript
disj = function (b, e, f){switch(arguments.length){case 1:return b;case 2:return a.call(this,
b,e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new
 F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.disj.a"></a>[function <span class="apidocSignatureSpan">mori.disj.</span>a (a, b)](#apidoc.element.mori.disj.a)
- description and source-code
```javascript
function a(a, b){return null==a?null:kb(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.disj.b"></a>[function <span class="apidocSignatureSpan">mori.disj.</span>b (a)](#apidoc.element.mori.disj.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.disj.d"></a>[function <span class="apidocSignatureSpan">mori.disj.</span>d (a, d, e)](#apidoc.element.mori.disj.d)
- description and source-code
```javascript
function c(a, d, e){for(;;){if(null==a)return null;a=b.a(a,d);if(t(e))d=G(e),e=K(e);else return a}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.disj.f"></a>[function <span class="apidocSignatureSpan">mori.disj.</span>f (a)](#apidoc.element.mori.disj.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var d=G(a);a=H(a);return c(b,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.disj.f1"></a>[function <span class="apidocSignatureSpan">mori.disj.</span>f1 (a)](#apidoc.element.mori.disj.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.disj.f2"></a>[function <span class="apidocSignatureSpan">mori.disj.</span>f2 (a, b)](#apidoc.element.mori.disj.f2)
- description and source-code
```javascript
function a(a, b){return null==a?null:kb(a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.dissoc"></a>[module mori.dissoc](#apidoc.module.mori.dissoc)

#### <a name="apidoc.element.mori.dissoc.dissoc"></a>[function <span class="apidocSignatureSpan">mori.</span>dissoc (b, e, f)](#apidoc.element.mori.dissoc.dissoc)
- description and source-code
```javascript
dissoc = function (b, e, f){switch(arguments.length){case 1:return b;case 2:return a.call(this,b,e);
default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,
0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dissoc.a"></a>[function <span class="apidocSignatureSpan">mori.dissoc.</span>a (a, b)](#apidoc.element.mori.dissoc.a)
- description and source-code
```javascript
function a(a, b){return null==a?null:eb(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dissoc.b"></a>[function <span class="apidocSignatureSpan">mori.dissoc.</span>b (a)](#apidoc.element.mori.dissoc.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dissoc.d"></a>[function <span class="apidocSignatureSpan">mori.dissoc.</span>d (a, d, e)](#apidoc.element.mori.dissoc.d)
- description and source-code
```javascript
function c(a, d, e){for(;;){if(null==a)return null;a=b.a(a,d);if(t(e))d=G(e),e=K(e);else return a}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dissoc.f"></a>[function <span class="apidocSignatureSpan">mori.dissoc.</span>f (a)](#apidoc.element.mori.dissoc.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var d=G(a);a=H(a);return c(b,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dissoc.f1"></a>[function <span class="apidocSignatureSpan">mori.dissoc.</span>f1 (a)](#apidoc.element.mori.dissoc.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dissoc.f2"></a>[function <span class="apidocSignatureSpan">mori.dissoc.</span>f2 (a, b)](#apidoc.element.mori.dissoc.f2)
- description and source-code
```javascript
function a(a, b){return null==a?null:eb(a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.drop"></a>[module mori.drop](#apidoc.module.mori.drop)

#### <a name="apidoc.element.mori.drop.drop"></a>[function <span class="apidocSignatureSpan">mori.</span>drop (c, e)](#apidoc.element.mori.drop.drop)
- description and source-code
```javascript
drop = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.drop.a"></a>[function <span class="apidocSignatureSpan">mori.drop.</span>a (a, b)](#apidoc.element.mori.drop.a)
- description and source-code
```javascript
function a(a, b){return new V(null,function(c){return function(){return c(a,b)}}(function(a,b){for(;;){var c=D(b);if(0<a&&c){var
d=a-1,c=H(c);a=d;b=c}else return c}}),null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.drop.b"></a>[function <span class="apidocSignatureSpan">mori.drop.</span>b (a)](#apidoc.element.mori.drop.b)
- description and source-code
```javascript
function b(a){return function(b){return function(a){return function(){function c(d,g){var h=qb(a);a.bb(0,a.Ra(null)-1);return 0<
h?d:b.a?b.a(d,g):b.call(null,d,g)}function d(a){return b.b?b.b(a):b.call(null,a)}function l(){return b.l?
b.l():b.call(null)}var m=null,m=function(a,b){switch(arguments.length){case 0:return l.call(this);case 1:return d.call(this,a);case
 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};m.l=l;m.b=d;m.a=c;return m}()}(new Me(a))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.drop.f1"></a>[function <span class="apidocSignatureSpan">mori.drop.</span>f1 (a)](#apidoc.element.mori.drop.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(a){return function(){function c(d,g){var h=qb(a);a.bb(0,a.Ra(null)-1);return 0<
h?d:b.a?b.a(d,g):b.call(null,d,g)}function d(a){return b.b?b.b(a):b.call(null,a)}function l(){return b.l?
b.l():b.call(null)}var m=null,m=function(a,b){switch(arguments.length){case 0:return l.call(this);case 1:return d.call(this,a);case
 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};m.l=l;m.b=d;m.a=c;return m}()}(new Me(a))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.drop.f2"></a>[function <span class="apidocSignatureSpan">mori.drop.</span>f2 (a, b)](#apidoc.element.mori.drop.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,function(c){return function(){return c(a,b)}}(function(a,b){for(;;){var c=D(b);if(0<a&&c){var
d=a-1,c=H(c);a=d;b=c}else return c}}),null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.dropWhile"></a>[module mori.dropWhile](#apidoc.module.mori.dropWhile)

#### <a name="apidoc.element.mori.dropWhile.dropWhile"></a>[function <span class="apidocSignatureSpan">mori.</span>dropWhile (c, e)](#apidoc.element.mori.dropWhile.dropWhile)
- description and source-code
```javascript
dropWhile = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dropWhile.a"></a>[function <span class="apidocSignatureSpan">mori.dropWhile.</span>a (a, b)](#apidoc.element.mori.dropWhile.a)
- description and source-code
```javascript
function a(a, b){return new V(null,function(c){return function(){return c(a,
b)}}(function(a,b){for(;;){var c=D(b),d;if(d=c)d=G(c),d=a.b?a.b(d):a.call(null,d);if(t(d))d=a,c=H(c),a=d,b=c;else return c}}),null
,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dropWhile.b"></a>[function <span class="apidocSignatureSpan">mori.dropWhile.</span>b (a)](#apidoc.element.mori.dropWhile.b)
- description and source-code
```javascript
function b(a){return function(b){return function(c){return function(){function g(g,h){var l=qb(c);if(t(t(l)?a.b?a.b(h):a.call(null
,h):l))return g;ac(c,null);return b.a?b.a(g,h):b.call(null,g,h)}function h(a){return b.b?b.b(a):b.call(null,a)}function l(){return
 b.l?b.l():b.call(null)}var m=null,m=function(a,b){switch(arguments.length){case 0:return l.call(this);case 1:return h.call(this
,
a);case 2:return g.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};m.l=l;m.b=h;m.a=g;return m}()}(new Me(!0))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dropWhile.f1"></a>[function <span class="apidocSignatureSpan">mori.dropWhile.</span>f1 (a)](#apidoc.element.mori.dropWhile.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(c){return function(){function g(g,h){var l=qb(c);if(t(t(l)?a.b?a.b(h):a.call(null
,h):l))return g;ac(c,null);return b.a?b.a(g,h):b.call(null,g,h)}function h(a){return b.b?b.b(a):b.call(null,a)}function l(){return
 b.l?b.l():b.call(null)}var m=null,m=function(a,b){switch(arguments.length){case 0:return l.call(this);case 1:return h.call(this
,
a);case 2:return g.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};m.l=l;m.b=h;m.a=g;return m}()}(new Me(!0))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.dropWhile.f2"></a>[function <span class="apidocSignatureSpan">mori.dropWhile.</span>f2 (a, b)](#apidoc.element.mori.dropWhile.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,function(c){return function(){return c(a,
b)}}(function(a,b){for(;;){var c=D(b),d;if(d=c)d=G(c),d=a.b?a.b(d):a.call(null,d);if(t(d))d=a,c=H(c),a=d,b=c;else return c}}),null
,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.equals"></a>[module mori.equals](#apidoc.module.mori.equals)

#### <a name="apidoc.element.mori.equals.equals"></a>[function <span class="apidocSignatureSpan">mori.</span>equals (b, e, f)](#apidoc.element.mori.equals.equals)
- description and source-code
```javascript
equals = function (b, e, f){switch(arguments.length){case 1:return!0;
case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g
]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.equals.a"></a>[function <span class="apidocSignatureSpan">mori.equals.</span>a (a, b)](#apidoc.element.mori.equals.a)
- description and source-code
```javascript
function a(a, b){return null==a?null==b:a===b||yb(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.equals.b"></a>[function <span class="apidocSignatureSpan">mori.equals.</span>b ()](#apidoc.element.mori.equals.b)
- description and source-code
```javascript
b = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.equals.d"></a>[function <span class="apidocSignatureSpan">mori.equals.</span>d (a, d, e)](#apidoc.element.mori.equals.d)
- description and source-code
```javascript
function c(a, d, e){for(;;)if(b.a(a,d))if(K(e))a=d,d=G(e),e=K(e);else return b.a(d,G(e));else return!1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.equals.f"></a>[function <span class="apidocSignatureSpan">mori.equals.</span>f (a)](#apidoc.element.mori.equals.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var d=G(a);a=H(a);return c(b,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.equals.f1"></a>[function <span class="apidocSignatureSpan">mori.equals.</span>f1 ()](#apidoc.element.mori.equals.f1)
- description and source-code
```javascript
f1 = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.equals.f2"></a>[function <span class="apidocSignatureSpan">mori.equals.</span>f2 (a, b)](#apidoc.element.mori.equals.f2)
- description and source-code
```javascript
function a(a, b){return null==a?null==b:a===b||yb(a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.filter"></a>[module mori.filter](#apidoc.module.mori.filter)

#### <a name="apidoc.element.mori.filter.filter"></a>[function <span class="apidocSignatureSpan">mori.</span>filter (c, e)](#apidoc.element.mori.filter.filter)
- description and source-code
```javascript
filter = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.filter.a"></a>[function <span class="apidocSignatureSpan">mori.filter.</span>a (a, b)](#apidoc.element.mori.filter.a)
- description and source-code
```javascript
function a(a, b){return new V(null,
function(){var f=D(b);if(f){if(fd(f)){for(var g=Yb(f),h=Q(g),l=Td(h),m=0;;)if(m<h){var p;p=C.a(g,m);p=a.b?a.b(p):a.call(null,p);
t(p)&&(p=C.a(g,m),l.add(p));m+=1}else break;return Wd(l.ca(),c.a(a,Zb(f)))}g=G(f);f=H(f);return t(a.b?a.b(g):a.call(null,g))?M(g
,c.a(a,f)):c.a(a,f)}return null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.filter.b"></a>[function <span class="apidocSignatureSpan">mori.filter.</span>b (a)](#apidoc.element.mori.filter.b)
- description and source-code
```javascript
function b(a){return function(b){return function(){function c(f,g){return t(a.b?a.b(g):a.call(null,g))?b.a?b.a(f,g):b.call(null,
f,g):f}function g(a){return b.b?b.b(a):b.call(null,a)}function h(){return b.l?
b.l():b.call(null)}var l=null,l=function(a,b){switch(arguments.length){case 0:return h.call(this);case 1:return g.call(this,a);case
 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};l.l=h;l.b=g;l.a=c;return l}()}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.filter.f1"></a>[function <span class="apidocSignatureSpan">mori.filter.</span>f1 (a)](#apidoc.element.mori.filter.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(){function c(f,g){return t(a.b?a.b(g):a.call(null,g))?b.a?b.a(f,g):b.call(null,
f,g):f}function g(a){return b.b?b.b(a):b.call(null,a)}function h(){return b.l?
b.l():b.call(null)}var l=null,l=function(a,b){switch(arguments.length){case 0:return h.call(this);case 1:return g.call(this,a);case
 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};l.l=h;l.b=g;l.a=c;return l}()}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.filter.f2"></a>[function <span class="apidocSignatureSpan">mori.filter.</span>f2 (a, b)](#apidoc.element.mori.filter.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,
function(){var f=D(b);if(f){if(fd(f)){for(var g=Yb(f),h=Q(g),l=Td(h),m=0;;)if(m<h){var p;p=C.a(g,m);p=a.b?a.b(p):a.call(null,p);
t(p)&&(p=C.a(g,m),l.add(p));m+=1}else break;return Wd(l.ca(),c.a(a,Zb(f)))}g=G(f);f=H(f);return t(a.b?a.b(g):a.call(null,g))?M(g
,c.a(a,f)):c.a(a,f)}return null},null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.fnil"></a>[module mori.fnil](#apidoc.module.mori.fnil)

#### <a name="apidoc.element.mori.fnil.fnil"></a>[function <span class="apidocSignatureSpan">mori.</span>fnil (d, f, g, h)](#apidoc.element.mori.fnil.fnil)
- description and source-code
```javascript
fnil = function (d, f, g, h){switch(arguments.length){case 2:return c.call(this,d,f);case 3:return b.call(this,d,f,g);case 4:return a.call
(this,d,f,g,h)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.fnil.a"></a>[function <span class="apidocSignatureSpan">mori.fnil.</span>a (a, b)](#apidoc.element.mori.fnil.a)
- description and source-code
```javascript
function c(a, b){return function(){function c(d,g,h){d=null==d?b:d;return a.c?a.c(d,g,h):a.call(null,d,g,h)}function d(c,g){var h
=null==c?b:c;return a.a?a.a(h,g):a.call(null,h,g)}function l(c){c=null==c?b:c;return a.b?a.b(c):a.call(null,c)}var m=null,p=function
(){function c(a,b,e,f){var g=null;if(3<arguments.length){for(var g=0,h=Array(arguments.length-3);g<h.length;)h[g]=arguments[g+3],++
g;g=new F(h,
0)}return d.call(this,a,b,e,g)}function d(c,g,h,l){return T.r(a,null==c?b:c,g,h,l)}c.i=3;c.f=function(a){var b=G(a);a=K(a);var c
=G(a);a=K(a);var e=G(a);a=H(a);return d(b,c,e,a)};c.d=d;return c}(),m=function(a,b,e,f){switch(arguments.length){case 1:return l
.call(this,a);case 2:return d.call(this,a,b);case 3:return c.call(this,a,b,e);default:var m=null;if(3<arguments.length){for(var
m=0,B=Array(arguments.length-3);m<B.length;)B[m]=arguments[m+3],++m;m=new F(B,0)}return p.d(a,b,e,m)}throw Error("Invalid arity: "+
arguments.length);};m.i=3;m.f=p.f;m.b=l;m.a=d;m.c=c;m.d=p.d;return m}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.fnil.c"></a>[function <span class="apidocSignatureSpan">mori.fnil.</span>c (a, b, c)](#apidoc.element.mori.fnil.c)
- description and source-code
```javascript
function b(a, b, c){return function(){function d(h,l,m){h=null==h?b:h;l=null==l?c:l;return a.c?a.c(h,l,m):a.call(null,h,l,m)}function
 l(d,h){var l=null==d?b:d,m=null==h?c:h;return a.a?a.a(l,m):a.call(null,l,m)}var m=null,p=function(){function d(a,b,c,e){var f=null
;if(3<arguments.length){for(var f=0,g=Array(arguments.length-
3);f<g.length;)g[f]=arguments[f+3],++f;f=new F(g,0)}return h.call(this,a,b,c,f)}function h(d,l,m,p){return T.r(a,null==d?b:d,null
==l?c:l,m,p)}d.i=3;d.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return h(b,c,d,a)};d.d=h;return d}(),m=
function(a,b,c,e){switch(arguments.length){case 2:return l.call(this,a,b);case 3:return d.call(this,a,b,c);default:var f=null;if
(3<arguments.length){for(var f=0,g=Array(arguments.length-3);f<g.length;)g[f]=arguments[f+3],++f;f=new F(g,0)}return p.d(a,
b,c,f)}throw Error("Invalid arity: "+arguments.length);};m.i=3;m.f=p.f;m.a=l;m.c=d;m.d=p.d;return m}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.fnil.f2"></a>[function <span class="apidocSignatureSpan">mori.fnil.</span>f2 (a, b)](#apidoc.element.mori.fnil.f2)
- description and source-code
```javascript
function c(a, b){return function(){function c(d,g,h){d=null==d?b:d;return a.c?a.c(d,g,h):a.call(null,d,g,h)}function d(c,g){var h
=null==c?b:c;return a.a?a.a(h,g):a.call(null,h,g)}function l(c){c=null==c?b:c;return a.b?a.b(c):a.call(null,c)}var m=null,p=function
(){function c(a,b,e,f){var g=null;if(3<arguments.length){for(var g=0,h=Array(arguments.length-3);g<h.length;)h[g]=arguments[g+3],++
g;g=new F(h,
0)}return d.call(this,a,b,e,g)}function d(c,g,h,l){return T.r(a,null==c?b:c,g,h,l)}c.i=3;c.f=function(a){var b=G(a);a=K(a);var c
=G(a);a=K(a);var e=G(a);a=H(a);return d(b,c,e,a)};c.d=d;return c}(),m=function(a,b,e,f){switch(arguments.length){case 1:return l
.call(this,a);case 2:return d.call(this,a,b);case 3:return c.call(this,a,b,e);default:var m=null;if(3<arguments.length){for(var
m=0,B=Array(arguments.length-3);m<B.length;)B[m]=arguments[m+3],++m;m=new F(B,0)}return p.d(a,b,e,m)}throw Error("Invalid arity: "+
arguments.length);};m.i=3;m.f=p.f;m.b=l;m.a=d;m.c=c;m.d=p.d;return m}()}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.fnil.f3"></a>[function <span class="apidocSignatureSpan">mori.fnil.</span>f3 (a, b, c)](#apidoc.element.mori.fnil.f3)
- description and source-code
```javascript
function b(a, b, c){return function(){function d(h,l,m){h=null==h?b:h;l=null==l?c:l;return a.c?a.c(h,l,m):a.call(null,h,l,m)}function
 l(d,h){var l=null==d?b:d,m=null==h?c:h;return a.a?a.a(l,m):a.call(null,l,m)}var m=null,p=function(){function d(a,b,c,e){var f=null
;if(3<arguments.length){for(var f=0,g=Array(arguments.length-
3);f<g.length;)g[f]=arguments[f+3],++f;f=new F(g,0)}return h.call(this,a,b,c,f)}function h(d,l,m,p){return T.r(a,null==d?b:d,null
==l?c:l,m,p)}d.i=3;d.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return h(b,c,d,a)};d.d=h;return d}(),m=
function(a,b,c,e){switch(arguments.length){case 2:return l.call(this,a,b);case 3:return d.call(this,a,b,c);default:var f=null;if
(3<arguments.length){for(var f=0,g=Array(arguments.length-3);f<g.length;)g[f]=arguments[f+3],++f;f=new F(g,0)}return p.d(a,
b,c,f)}throw Error("Invalid arity: "+arguments.length);};m.i=3;m.f=p.f;m.a=l;m.c=d;m.d=p.d;return m}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.fnil.f4"></a>[function <span class="apidocSignatureSpan">mori.fnil.</span>f4 (a, b, c, d)](#apidoc.element.mori.fnil.f4)
- description and source-code
```javascript
function a(a, b, c, d){return function(){function l(l,m,p){l=null==l?b:l;m=null==m?c:m;p=null==p?d:p;return a.c?a.c(l,m,p):a.call(null
,l,m,p)}function m(d,h){var l=null==d?b:d,m=null==h?c:h;return a.a?a.a(l,m):a.call(null,l,m)}var p=null,q=function(){function l(
a,
b,c,d){var e=null;if(3<arguments.length){for(var e=0,f=Array(arguments.length-3);e<f.length;)f[e]=arguments[e+3],++e;e=new F(f,0
)}return m.call(this,a,b,c,e)}function m(l,p,q,s){return T.r(a,null==l?b:l,null==p?c:p,null==q?d:q,s)}l.i=3;l.f=function(a){var
b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return m(b,c,d,a)};l.d=m;return l}(),p=function(a,b,c,d){switch(arguments.length
){case 2:return m.call(this,a,b);case 3:return l.call(this,a,b,c);default:var e=null;if(3<arguments.length){for(var e=
0,f=Array(arguments.length-3);e<f.length;)f[e]=arguments[e+3],++e;e=new F(f,0)}return q.d(a,b,c,e)}throw Error("Invalid arity: "+
arguments.length);};p.i=3;p.f=q.f;p.a=m;p.c=l;p.d=q.d;return p}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.fnil.n"></a>[function <span class="apidocSignatureSpan">mori.fnil.</span>n (a, b, c, d)](#apidoc.element.mori.fnil.n)
- description and source-code
```javascript
function a(a, b, c, d){return function(){function l(l,m,p){l=null==l?b:l;m=null==m?c:m;p=null==p?d:p;return a.c?a.c(l,m,p):a.call(null
,l,m,p)}function m(d,h){var l=null==d?b:d,m=null==h?c:h;return a.a?a.a(l,m):a.call(null,l,m)}var p=null,q=function(){function l(
a,
b,c,d){var e=null;if(3<arguments.length){for(var e=0,f=Array(arguments.length-3);e<f.length;)f[e]=arguments[e+3],++e;e=new F(f,0
)}return m.call(this,a,b,c,e)}function m(l,p,q,s){return T.r(a,null==l?b:l,null==p?c:p,null==q?d:q,s)}l.i=3;l.f=function(a){var
b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return m(b,c,d,a)};l.d=m;return l}(),p=function(a,b,c,d){switch(arguments.length
){case 2:return m.call(this,a,b);case 3:return l.call(this,a,b,c);default:var e=null;if(3<arguments.length){for(var e=
0,f=Array(arguments.length-3);e<f.length;)f[e]=arguments[e+3],++e;e=new F(f,0)}return q.d(a,b,c,e)}throw Error("Invalid arity: "+
arguments.length);};p.i=3;p.f=q.f;p.a=m;p.c=l;p.d=q.d;return p}()}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.get"></a>[module mori.get](#apidoc.module.mori.get)

#### <a name="apidoc.element.mori.get.get"></a>[function <span class="apidocSignatureSpan">mori.</span>get (c, e, f)](#apidoc.element.mori.get.get)
- description and source-code
```javascript
get = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,
c,e,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
return the proposed mutable iterators:

'''javascript
var m = mori;
var h = m.hashMap("foo", 1, "bar", 2);

h.has("foo"); // => true
h.get("foo"); // => 1

var iter = h.keys();
iter.next(); // => {done: false, value: "foo"}
'''

This feature is subject to changes in the ES6 proposal.
...
```

#### <a name="apidoc.element.mori.get.a"></a>[function <span class="apidocSignatureSpan">mori.get.</span>a (a, b)](#apidoc.element.mori.get.a)
- description and source-code
```javascript
function b(a, b){return null==a?null:a&&(a.j&256||a.Rb)?a.t(null,b):a instanceof Array?b<a.length?a[b]:null:"string"===typeof a?b
<a.length?a[b]:null:w(Za,a)?$a.a(a,b):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.get.c"></a>[function <span class="apidocSignatureSpan">mori.get.</span>c (a, b, c)](#apidoc.element.mori.get.c)
- description and source-code
```javascript
function a(a, b, c){return null!=a?a&&(a.j&256||a.Rb)?a.s(null,b,c):a instanceof Array?b<a.length?a[b]:c:"string"===typeof a?b<a.length
?a[b]:c:w(Za,a)?$a.c(a,b,c):c:c}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.get.f2"></a>[function <span class="apidocSignatureSpan">mori.get.</span>f2 (a, b)](#apidoc.element.mori.get.f2)
- description and source-code
```javascript
function b(a, b){return null==a?null:a&&(a.j&256||a.Rb)?a.t(null,b):a instanceof Array?b<a.length?a[b]:null:"string"===typeof a?b
<a.length?a[b]:null:w(Za,a)?$a.a(a,b):null}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.get.f3"></a>[function <span class="apidocSignatureSpan">mori.get.</span>f3 (a, b, c)](#apidoc.element.mori.get.f3)
- description and source-code
```javascript
function a(a, b, c){return null!=a?a&&(a.j&256||a.Rb)?a.s(null,b,c):a instanceof Array?b<a.length?a[b]:c:"string"===typeof a?b<a.length
?a[b]:c:w(Za,a)?$a.c(a,b,c):c:c}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.getIn"></a>[module mori.getIn](#apidoc.module.mori.getIn)

#### <a name="apidoc.element.mori.getIn.getIn"></a>[function <span class="apidocSignatureSpan">mori.</span>getIn (c, e, f)](#apidoc.element.mori.getIn.getIn)
- description and source-code
```javascript
getIn = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.getIn.a"></a>[function <span class="apidocSignatureSpan">mori.getIn.</span>a (a, b)](#apidoc.element.mori.getIn.a)
- description and source-code
```javascript
function b(a, b){return c.c(a,b,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.getIn.c"></a>[function <span class="apidocSignatureSpan">mori.getIn.</span>c (a, b, c)](#apidoc.element.mori.getIn.c)
- description and source-code
```javascript
function a(a, b, c){var g=jd;for(b=D(b);;)if(b){var h=a;if(h?h.j&256||h.Rb||(h.j?0:w(Za,h)):w(Za,h)){a=S.c(a,G(b),g);if(g===a)return c;b=K(b)}else
 return c}else return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.getIn.f2"></a>[function <span class="apidocSignatureSpan">mori.getIn.</span>f2 (a, b)](#apidoc.element.mori.getIn.f2)
- description and source-code
```javascript
function b(a, b){return c.c(a,b,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.getIn.f3"></a>[function <span class="apidocSignatureSpan">mori.getIn.</span>f3 (a, b, c)](#apidoc.element.mori.getIn.f3)
- description and source-code
```javascript
function a(a, b, c){var g=jd;for(b=D(b);;)if(b){var h=a;if(h?h.j&256||h.Rb||(h.j?0:w(Za,h)):w(Za,h)){a=S.c(a,G(b),g);if(g===a)return c;b=K(b)}else
 return c}else return a}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.gt"></a>[module mori.gt](#apidoc.module.mori.gt)

#### <a name="apidoc.element.mori.gt.gt"></a>[function <span class="apidocSignatureSpan">mori.</span>gt (a, d, e)](#apidoc.element.mori.gt.gt)
- description and source-code
```javascript
gt = function (a, d, e){switch(arguments.length){case 1:return!0;case 2:return a>d;default:var f=null;if(2<arguments.length){for(var f=
0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gt.a"></a>[function <span class="apidocSignatureSpan">mori.gt.</span>a (a, b)](#apidoc.element.mori.gt.a)
- description and source-code
```javascript
a = function (a, b){return a>b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gt.b"></a>[function <span class="apidocSignatureSpan">mori.gt.</span>b ()](#apidoc.element.mori.gt.b)
- description and source-code
```javascript
b = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gt.d"></a>[function <span class="apidocSignatureSpan">mori.gt.</span>d (a, c, d)](#apidoc.element.mori.gt.d)
- description and source-code
```javascript
function b(a, c, d){for(;;)if(a>c)if(K(d))a=c,c=G(d),d=K(d);else return c>G(d);else return!1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gt.f"></a>[function <span class="apidocSignatureSpan">mori.gt.</span>f (a)](#apidoc.element.mori.gt.f)
- description and source-code
```javascript
f = function (a){var c=
G(a);a=K(a);var g=G(a);a=H(a);return b(c,g,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gt.f1"></a>[function <span class="apidocSignatureSpan">mori.gt.</span>f1 ()](#apidoc.element.mori.gt.f1)
- description and source-code
```javascript
f1 = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gt.f2"></a>[function <span class="apidocSignatureSpan">mori.gt.</span>f2 (a, b)](#apidoc.element.mori.gt.f2)
- description and source-code
```javascript
f2 = function (a, b){return a>b}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.gte"></a>[module mori.gte](#apidoc.module.mori.gte)

#### <a name="apidoc.element.mori.gte.gte"></a>[function <span class="apidocSignatureSpan">mori.</span>gte (a, d, e)](#apidoc.element.mori.gte.gte)
- description and source-code
```javascript
gte = function (a, d, e){switch(arguments.length){case 1:return!0;case 2:return a>=d;default:var f=null;if(2<arguments.length){for(var f
=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+
2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gte.a"></a>[function <span class="apidocSignatureSpan">mori.gte.</span>a (a, b)](#apidoc.element.mori.gte.a)
- description and source-code
```javascript
a = function (a, b){return a>=b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gte.b"></a>[function <span class="apidocSignatureSpan">mori.gte.</span>b ()](#apidoc.element.mori.gte.b)
- description and source-code
```javascript
b = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gte.d"></a>[function <span class="apidocSignatureSpan">mori.gte.</span>d (a, c, d)](#apidoc.element.mori.gte.d)
- description and source-code
```javascript
function b(a, c, d){for(;;)if(a>=c)if(K(d))a=c,c=G(d),d=K(d);else return c>=G(d);else return!1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gte.f"></a>[function <span class="apidocSignatureSpan">mori.gte.</span>f (a)](#apidoc.element.mori.gte.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var g=G(a);a=H(a);return b(c,g,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gte.f1"></a>[function <span class="apidocSignatureSpan">mori.gte.</span>f1 ()](#apidoc.element.mori.gte.f1)
- description and source-code
```javascript
f1 = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.gte.f2"></a>[function <span class="apidocSignatureSpan">mori.gte.</span>f2 (a, b)](#apidoc.element.mori.gte.f2)
- description and source-code
```javascript
f2 = function (a, b){return a>=b}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.hashMap"></a>[module mori.hashMap](#apidoc.module.mori.hashMap)

#### <a name="apidoc.element.mori.hashMap.hashMap"></a>[function <span class="apidocSignatureSpan">mori.</span>hashMap (a)](#apidoc.element.mori.hashMap.hashMap)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,
d)}
```
- example usage
```shell
...
[Set](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set)
interfaces. The main difference with the spec is that key lookup is
based on value not reference. 'keys', 'values', and 'entries' methods
return the proposed mutable iterators:

'''javascript
var m = mori;
var h = m.hashMap("foo", 1, "bar", 2);

h.has("foo"); // => true
h.get("foo"); // => 1

var iter = h.keys();
iter.next(); // => {done: false, value: "foo"}
'''
...
```

#### <a name="apidoc.element.mori.hashMap.d"></a>[function <span class="apidocSignatureSpan">mori.hashMap.</span>d (a)](#apidoc.element.mori.hashMap.d)
- description and source-code
```javascript
function b(a){a:{a=T.a(Ha,a);for(var b=a.length,e=0,f=Ob(Uf);;)if(e<b)var g=e+2,f=Rb(f,a[e],a[e+1]),e=g;else{a=Qb(f);break a}a=void
 0}return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.hashMap.f"></a>[function <span class="apidocSignatureSpan">mori.hashMap.</span>f (a)](#apidoc.element.mori.hashMap.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.interleave"></a>[module mori.interleave](#apidoc.module.mori.interleave)

#### <a name="apidoc.element.mori.interleave.interleave"></a>[function <span class="apidocSignatureSpan">mori.</span>interleave (b, e, f)](#apidoc.element.mori.interleave.interleave)
- description and source-code
```javascript
interleave = function (b, e, f){switch(arguments.length){case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length){for(var g=0,h
=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.interleave.a"></a>[function <span class="apidocSignatureSpan">mori.interleave.</span>a (a, c)](#apidoc.element.mori.interleave.a)
- description and source-code
```javascript
function a(a, c){return new V(null,function(){var f=
D(a),g=D(c);return f&&g?M(G(f),M(G(g),b.a(H(f),H(g)))):null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.interleave.d"></a>[function <span class="apidocSignatureSpan">mori.interleave.</span>d (a, d, e)](#apidoc.element.mori.interleave.d)
- description and source-code
```javascript
function c(a, d, e){return new V(null,function(){var c=Oe.a(D,Nc.d(e,d,Kc([a],0)));return Ee(ud,c)?ae.a(Oe.a(G,c),T.a(b,Oe.a(H,c))):
null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.interleave.f"></a>[function <span class="apidocSignatureSpan">mori.interleave.</span>f (a)](#apidoc.element.mori.interleave.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var d=G(a);a=H(a);return c(b,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.interleave.f2"></a>[function <span class="apidocSignatureSpan">mori.interleave.</span>f2 (a, c)](#apidoc.element.mori.interleave.f2)
- description and source-code
```javascript
function a(a, c){return new V(null,function(){var f=
D(a),g=D(c);return f&&g?M(G(f),M(G(g),b.a(H(f),H(g)))):null},null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.intersection"></a>[module mori.intersection](#apidoc.module.mori.intersection)

#### <a name="apidoc.element.mori.intersection.intersection"></a>[function <span class="apidocSignatureSpan">mori.</span>intersection (b, e, f)](#apidoc.element.mori.intersection.intersection)
- description and source-code
```javascript
intersection = function (b, e, f){switch(arguments.length){case 1:return b;case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length
){for(var g=0,h=Array(arguments.length-
2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intersection.a"></a>[function <span class="apidocSignatureSpan">mori.intersection.</span>a (a, b)](#apidoc.element.mori.intersection.a)
- description and source-code
```javascript
function a(a, b){for(;;)if(Q(b)<Q(a)){var c=a;a=b;b=c}else return A.c(function(a,b){return function(a,c){return nd(b,c)?a:Xc.a(a,
c)}}(a,b),a,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intersection.b"></a>[function <span class="apidocSignatureSpan">mori.intersection.</span>b (a)](#apidoc.element.mori.intersection.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intersection.d"></a>[function <span class="apidocSignatureSpan">mori.intersection.</span>d (a, d, e)](#apidoc.element.mori.intersection.d)
- description and source-code
```javascript
function c(a, d, e){a=Qh(function(a){return-Q(a)},Nc.d(e,d,Kc([a],0)));return A.c(b,G(a),H(a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intersection.f"></a>[function <span class="apidocSignatureSpan">mori.intersection.</span>f (a)](#apidoc.element.mori.intersection.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var d=G(a);a=H(a);return c(b,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intersection.f1"></a>[function <span class="apidocSignatureSpan">mori.intersection.</span>f1 (a)](#apidoc.element.mori.intersection.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intersection.f2"></a>[function <span class="apidocSignatureSpan">mori.intersection.</span>f2 (a, b)](#apidoc.element.mori.intersection.f2)
- description and source-code
```javascript
function a(a, b){for(;;)if(Q(b)<Q(a)){var c=a;a=b;b=c}else return A.c(function(a,b){return function(a,c){return nd(b,c)?a:Xc.a(a,
c)}}(a,b),a,a)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.into"></a>[module mori.into](#apidoc.module.mori.into)

#### <a name="apidoc.element.mori.into.into"></a>[function <span class="apidocSignatureSpan">mori.</span>into (c, e, f)](#apidoc.element.mori.into.into)
- description and source-code
```javascript
into = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
...
var a = [];

for(var i = 0; i < 1000000; i++) {
  a.push(i);
}

// make it immutable
var v = m.into(m.vector(), a);

function time(f) {
  var s = new Date();
  f();
  console.log(((new Date())-s)+"ms");
}
...
```

#### <a name="apidoc.element.mori.into.a"></a>[function <span class="apidocSignatureSpan">mori.into.</span>a (a, b)](#apidoc.element.mori.into.a)
- description and source-code
```javascript
function b(a, b){return null!=a?a&&(a.q&4||a.dc)?O(ce(A.c(Pb,Ob(a),b)),Vc(a)):A.c(Ra,a,b):A.c(Nc,J,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.into.c"></a>[function <span class="apidocSignatureSpan">mori.into.</span>c (a, b, c)](#apidoc.element.mori.into.c)
- description and source-code
```javascript
function a(a, b, c){return a&&(a.q&4||a.dc)?O(ce(wd.n(b,de,Ob(a),c)),Vc(a)):wd.n(b,Nc,a,c)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.into.f2"></a>[function <span class="apidocSignatureSpan">mori.into.</span>f2 (a, b)](#apidoc.element.mori.into.f2)
- description and source-code
```javascript
function b(a, b){return null!=a?a&&(a.q&4||a.dc)?O(ce(A.c(Pb,Ob(a),b)),Vc(a)):A.c(Ra,a,b):A.c(Nc,J,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.into.f3"></a>[function <span class="apidocSignatureSpan">mori.into.</span>f3 (a, b, c)](#apidoc.element.mori.into.f3)
- description and source-code
```javascript
function a(a, b, c){return a&&(a.q&4||a.dc)?O(ce(wd.n(b,de,Ob(a),c)),Vc(a)):wd.n(b,Nc,a,c)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.intoArray"></a>[module mori.intoArray](#apidoc.module.mori.intoArray)

#### <a name="apidoc.element.mori.intoArray.intoArray"></a>[function <span class="apidocSignatureSpan">mori.</span>intoArray (d, c)](#apidoc.element.mori.intoArray.intoArray)
- description and source-code
```javascript
intoArray = function (d, c){switch(arguments.length){case 1:return b.call(this,d);case 2:return a.call(this,0,c)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
...
You can use it from your projects like so:

'''javascript
var inc = function(n) {
  return n+1;
};

mori.intoArray(mori.map(inc, mori.vector(1,2,3,4,5)));
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
...
```

#### <a name="apidoc.element.mori.intoArray.a"></a>[function <span class="apidocSignatureSpan">mori.intoArray.</span>a (a, b)](#apidoc.element.mori.intoArray.a)
- description and source-code
```javascript
function a(a, b){function c(a,b){a.push(b);return a}var g=[];return A.c?A.c(c,g,b):A.call(null,c,g,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intoArray.b"></a>[function <span class="apidocSignatureSpan">mori.intoArray.</span>b (a)](#apidoc.element.mori.intoArray.b)
- description and source-code
```javascript
function b(a){return c.a(null,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intoArray.f1"></a>[function <span class="apidocSignatureSpan">mori.intoArray.</span>f1 (a)](#apidoc.element.mori.intoArray.f1)
- description and source-code
```javascript
function b(a){return c.a(null,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.intoArray.f2"></a>[function <span class="apidocSignatureSpan">mori.intoArray.</span>f2 (a, b)](#apidoc.element.mori.intoArray.f2)
- description and source-code
```javascript
function a(a, b){function c(a,b){a.push(b);return a}var g=[];return A.c?A.c(c,g,b):A.call(null,c,g,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.join"></a>[module mori.join](#apidoc.module.mori.join)

#### <a name="apidoc.element.mori.join.join"></a>[function <span class="apidocSignatureSpan">mori.</span>join (c, e, f)](#apidoc.element.mori.join.join)
- description and source-code
```javascript
join = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.join.a"></a>[function <span class="apidocSignatureSpan">mori.join.</span>a (a, b)](#apidoc.element.mori.join.a)
- description and source-code
```javascript
function b(a, b){if(D(a)&&D(b)){var c=Sh.a(fh(Tg(G(a))),fh(Tg(G(b)))),
g=Q(a)<=Q(b)?new W(null,2,5,uf,[a,b],null):new W(null,2,5,uf,[b,a],null),h=R.c(g,0,null),l=R.c(g,1,null),m=Vh(h,c);return A.c(function
(a,b,c,d,e){return function(f,g){var h=function(){var b=Yg(g,a);return e.b?e.b(b):e.call(null,b)}();return t(h)?A.c(function(){return
 function(a,b){return Nc.a(a,Wg.d(Kc([b,g],0)))}}(h,a,b,c,d,e),f,h):f}}(c,g,h,l,m),bh,l)}return bh}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.join.c"></a>[function <span class="apidocSignatureSpan">mori.join.</span>c (a, b, c)](#apidoc.element.mori.join.c)
- description and source-code
```javascript
function a(a, b, c){a=Q(a)<=Q(b)?new W(null,3,5,uf,[a,b,Wh(c)],null):new W(null,3,5,uf,[b,a,c],null);b=R.c(a,0,null);c=R.c(a,1,null
);var g=R.c(a,2,null),h=Vh(b,Vg(g));return A.c(function(a,b,c,d,e){return function(f,g){var h=function(){var a=Uh(Yg(g,Tg(d)),d);
return e.b?e.b(a):e.call(null,a)}();return t(h)?A.c(function(){return function(a,b){return Nc.a(a,Wg.d(Kc([b,g],0)))}}(h,a,b,c,d
,e),f,h):f}}(a,b,c,g,h),bh,c)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.join.f2"></a>[function <span class="apidocSignatureSpan">mori.join.</span>f2 (a, b)](#apidoc.element.mori.join.f2)
- description and source-code
```javascript
function b(a, b){if(D(a)&&D(b)){var c=Sh.a(fh(Tg(G(a))),fh(Tg(G(b)))),
g=Q(a)<=Q(b)?new W(null,2,5,uf,[a,b],null):new W(null,2,5,uf,[b,a],null),h=R.c(g,0,null),l=R.c(g,1,null),m=Vh(h,c);return A.c(function
(a,b,c,d,e){return function(f,g){var h=function(){var b=Yg(g,a);return e.b?e.b(b):e.call(null,b)}();return t(h)?A.c(function(){return
 function(a,b){return Nc.a(a,Wg.d(Kc([b,g],0)))}}(h,a,b,c,d,e),f,h):f}}(c,g,h,l,m),bh,l)}return bh}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.join.f3"></a>[function <span class="apidocSignatureSpan">mori.join.</span>f3 (a, b, c)](#apidoc.element.mori.join.f3)
- description and source-code
```javascript
function a(a, b, c){a=Q(a)<=Q(b)?new W(null,3,5,uf,[a,b,Wh(c)],null):new W(null,3,5,uf,[b,a,c],null);b=R.c(a,0,null);c=R.c(a,1,null
);var g=R.c(a,2,null),h=Vh(b,Vg(g));return A.c(function(a,b,c,d,e){return function(f,g){var h=function(){var a=Uh(Yg(g,Tg(d)),d);
return e.b?e.b(a):e.call(null,a)}();return t(h)?A.c(function(){return function(a,b){return Nc.a(a,Wg.d(Kc([b,g],0)))}}(h,a,b,c,d
,e),f,h):f}}(a,b,c,g,h),bh,c)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.juxt"></a>[module mori.juxt](#apidoc.module.mori.juxt)

#### <a name="apidoc.element.mori.juxt.juxt"></a>[function <span class="apidocSignatureSpan">mori.</span>juxt (a)](#apidoc.element.mori.juxt.juxt)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.juxt.d"></a>[function <span class="apidocSignatureSpan">mori.juxt.</span>d (a)](#apidoc.element.mori.juxt.d)
- description and source-code
```javascript
function b(a){return function(){function b(a){var c=null;if(0<arguments.length){for(var c=0,d=Array(arguments.length-0);c<d.length
;)d[c]=arguments[c+0],++c;c=new F(d,0)}return e.call(this,c)}function e(b){var d=function(){function d(a){return T.a(a,b)}return
 Oe.a?Oe.a(d,a):Oe.call(null,d,a)}();return Ia.b?Ia.b(d):Ia.call(null,
d)}b.i=0;b.f=function(a){a=D(a);return e(a)};b.d=e;return b}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.juxt.f"></a>[function <span class="apidocSignatureSpan">mori.juxt.</span>f (a)](#apidoc.element.mori.juxt.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.keep"></a>[module mori.keep](#apidoc.module.mori.keep)

#### <a name="apidoc.element.mori.keep.keep"></a>[function <span class="apidocSignatureSpan">mori.</span>keep (c, e)](#apidoc.element.mori.keep.keep)
- description and source-code
```javascript
keep = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keep.a"></a>[function <span class="apidocSignatureSpan">mori.keep.</span>a (a, b)](#apidoc.element.mori.keep.a)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var f=D(b);if(f){if(fd(f)){for(var g=Yb(f),h=Q(g),l=Td(h),m=0;;)if(m<h){var p=function
(){var b=C.a(g,m);return a.b?a.b(b):a.call(null,b)}();
null!=p&&l.add(p);m+=1}else break;return Wd(l.ca(),c.a(a,Zb(f)))}h=function(){var b=G(f);return a.b?a.b(b):a.call(null,b)}();return
 null==h?c.a(a,H(f)):M(h,c.a(a,H(f)))}return null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keep.b"></a>[function <span class="apidocSignatureSpan">mori.keep.</span>b (a)](#apidoc.element.mori.keep.b)
- description and source-code
```javascript
function b(a){return function(b){return function(){function c(f,g){var h=a.b?a.b(g):a.call(null,g);return null==h?f:b.a?b.a(f,h):
b.call(null,f,h)}function g(a){return b.b?b.b(a):b.call(null,a)}function h(){return b.l?b.l():b.call(null)}var l=null,l=function
(a,b){switch(arguments.length){case 0:return h.call(this);
case 1:return g.call(this,a);case 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};l.l=h;l.b=g;l.a=c;
return l}()}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keep.f1"></a>[function <span class="apidocSignatureSpan">mori.keep.</span>f1 (a)](#apidoc.element.mori.keep.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(){function c(f,g){var h=a.b?a.b(g):a.call(null,g);return null==h?f:b.a?b.a(f,h):
b.call(null,f,h)}function g(a){return b.b?b.b(a):b.call(null,a)}function h(){return b.l?b.l():b.call(null)}var l=null,l=function
(a,b){switch(arguments.length){case 0:return h.call(this);
case 1:return g.call(this,a);case 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};l.l=h;l.b=g;l.a=c;
return l}()}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keep.f2"></a>[function <span class="apidocSignatureSpan">mori.keep.</span>f2 (a, b)](#apidoc.element.mori.keep.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var f=D(b);if(f){if(fd(f)){for(var g=Yb(f),h=Q(g),l=Td(h),m=0;;)if(m<h){var p=function
(){var b=C.a(g,m);return a.b?a.b(b):a.call(null,b)}();
null!=p&&l.add(p);m+=1}else break;return Wd(l.ca(),c.a(a,Zb(f)))}h=function(){var b=G(f);return a.b?a.b(b):a.call(null,b)}();return
 null==h?c.a(a,H(f)):M(h,c.a(a,H(f)))}return null},null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.keepIndexed"></a>[module mori.keepIndexed](#apidoc.module.mori.keepIndexed)

#### <a name="apidoc.element.mori.keepIndexed.keepIndexed"></a>[function <span class="apidocSignatureSpan">mori.</span>keepIndexed (c, e)](#apidoc.element.mori.keepIndexed.keepIndexed)
- description and source-code
```javascript
keepIndexed = function (c, e){switch(arguments.length){case 1:return b.call(this,
c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keepIndexed.a"></a>[function <span class="apidocSignatureSpan">mori.keepIndexed.</span>a (a, b)](#apidoc.element.mori.keepIndexed.a)
- description and source-code
```javascript
function a(a, b){return function g(b,c){return new V(null,function(){var e=D(c);if(e){if(fd(e)){for(var p=Yb(e),q=Q(p),s=Td(q),u=
0;;)if(u<q){var v=function(){var c=b+u,e=C.a(p,u);return a.a?a.a(c,e):a.call(null,c,e)}();null!=v&&s.add(v);u+=1}else break;return
 Wd(s.ca(),g(b+q,Zb(e)))}q=function(){var c=G(e);return a.a?a.a(b,c):a.call(null,b,c)}();return null==q?g(b+1,H(e)):M(q,g(b+1,H(
e)))}return null},null,null)}(0,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keepIndexed.b"></a>[function <span class="apidocSignatureSpan">mori.keepIndexed.</span>b (a)](#apidoc.element.mori.keepIndexed.b)
- description and source-code
```javascript
function b(a){return function(b){return function(c){return function(){function g(g,
h){var l=c.bb(0,c.Ra(null)+1),l=a.a?a.a(l,h):a.call(null,l,h);return null==l?g:b.a?b.a(g,l):b.call(null,g,l)}function h(a){return
 b.b?b.b(a):b.call(null,a)}function l(){return b.l?b.l():b.call(null)}var m=null,m=function(a,b){switch(arguments.length){case 0
:return l.call(this);case 1:return h.call(this,a);case 2:return g.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};
m.l=l;m.b=h;m.a=g;return m}()}(new Me(-1))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keepIndexed.f1"></a>[function <span class="apidocSignatureSpan">mori.keepIndexed.</span>f1 (a)](#apidoc.element.mori.keepIndexed.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(c){return function(){function g(g,
h){var l=c.bb(0,c.Ra(null)+1),l=a.a?a.a(l,h):a.call(null,l,h);return null==l?g:b.a?b.a(g,l):b.call(null,g,l)}function h(a){return
 b.b?b.b(a):b.call(null,a)}function l(){return b.l?b.l():b.call(null)}var m=null,m=function(a,b){switch(arguments.length){case 0
:return l.call(this);case 1:return h.call(this,a);case 2:return g.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};
m.l=l;m.b=h;m.a=g;return m}()}(new Me(-1))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keepIndexed.f2"></a>[function <span class="apidocSignatureSpan">mori.keepIndexed.</span>f2 (a, b)](#apidoc.element.mori.keepIndexed.f2)
- description and source-code
```javascript
function a(a, b){return function g(b,c){return new V(null,function(){var e=D(c);if(e){if(fd(e)){for(var p=Yb(e),q=Q(p),s=Td(q),u=
0;;)if(u<q){var v=function(){var c=b+u,e=C.a(p,u);return a.a?a.a(c,e):a.call(null,c,e)}();null!=v&&s.add(v);u+=1}else break;return
 Wd(s.ca(),g(b+q,Zb(e)))}q=function(){var c=G(e);return a.a?a.a(b,c):a.call(null,b,c)}();return null==q?g(b+1,H(e)):M(q,g(b+1,H(
e)))}return null},null,null)}(0,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.keyword"></a>[module mori.keyword](#apidoc.module.mori.keyword)

#### <a name="apidoc.element.mori.keyword.keyword"></a>[function <span class="apidocSignatureSpan">mori.</span>keyword (c, e)](#apidoc.element.mori.keyword.keyword)
- description and source-code
```javascript
keyword = function (c, e){switch(arguments.length){case 1:return b.call(this,
c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keyword.a"></a>[function <span class="apidocSignatureSpan">mori.keyword.</span>a (a, b)](#apidoc.element.mori.keyword.a)
- description and source-code
```javascript
function a(a, b){return new U(a,b,[z(t(a)?[z(a),z("/")].join(""):null),z(b)].join(""),null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keyword.b"></a>[function <span class="apidocSignatureSpan">mori.keyword.</span>b (a)](#apidoc.element.mori.keyword.b)
- description and source-code
```javascript
function b(a){if(a instanceof U)return a;if(a instanceof qc){var b;if(a&&(a.q&4096||a.lc))b=a.ba;else throw Error([z("Doesn't support
 namespace: "),z(a)].join(""));return new U(b,Od.b?Od.b(a):Od.call(null,a),a.ta,null)}return"string"===typeof a?(b=a.split("/"),
2===b.length?new U(b[0],b[1],a,null):new U(null,b[0],a,null)):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keyword.f1"></a>[function <span class="apidocSignatureSpan">mori.keyword.</span>f1 (a)](#apidoc.element.mori.keyword.f1)
- description and source-code
```javascript
function b(a){if(a instanceof U)return a;if(a instanceof qc){var b;if(a&&(a.q&4096||a.lc))b=a.ba;else throw Error([z("Doesn't support
 namespace: "),z(a)].join(""));return new U(b,Od.b?Od.b(a):Od.call(null,a),a.ta,null)}return"string"===typeof a?(b=a.split("/"),
2===b.length?new U(b[0],b[1],a,null):new U(null,b[0],a,null)):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.keyword.f2"></a>[function <span class="apidocSignatureSpan">mori.keyword.</span>f2 (a, b)](#apidoc.element.mori.keyword.f2)
- description and source-code
```javascript
function a(a, b){return new U(a,b,[z(t(a)?[z(a),z("/")].join(""):null),z(b)].join(""),null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.knit"></a>[module mori.knit](#apidoc.module.mori.knit)

#### <a name="apidoc.element.mori.knit.knit"></a>[function <span class="apidocSignatureSpan">mori.</span>knit (a)](#apidoc.element.mori.knit.knit)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.knit.d"></a>[function <span class="apidocSignatureSpan">mori.knit.</span>d (a)](#apidoc.element.mori.knit.d)
- description and source-code
```javascript
function b(a){return function(b){var e=function(){function e(a,b){return a.b?a.b(b):a.call(null,b)}return Oe.c?Oe.c(e,a,b):Oe.call
(null,e,a,b)}();return Ia.b?Ia.b(e):Ia.call(null,e)}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.knit.f"></a>[function <span class="apidocSignatureSpan">mori.knit.</span>f (a)](#apidoc.element.mori.knit.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.list"></a>[module mori.list](#apidoc.module.mori.list)

#### <a name="apidoc.element.mori.list.list"></a>[function <span class="apidocSignatureSpan">mori.</span>list (a)](#apidoc.element.mori.list.list)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.list.d"></a>[function <span class="apidocSignatureSpan">mori.list.</span>d (a)](#apidoc.element.mori.list.d)
- description and source-code
```javascript
function b(a){var b;if(a instanceof F&&0===a.m)b=a.e;else a:{for(b=[];;)if(null!=a)b.push(a.N(null)),a=a.T(null);else break a;b=
void 0}a=b.length;for(var e=J;;)if(0<a){var f=a-1,e=e.G(null,b[a-1]);a=f}else return e}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.list.f"></a>[function <span class="apidocSignatureSpan">mori.list.</span>f (a)](#apidoc.element.mori.list.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.lt"></a>[module mori.lt](#apidoc.module.mori.lt)

#### <a name="apidoc.element.mori.lt.lt"></a>[function <span class="apidocSignatureSpan">mori.</span>lt (a, d, e)](#apidoc.element.mori.lt.lt)
- description and source-code
```javascript
lt = function (a, d, e){switch(arguments.length){case 1:return!0;case 2:return a<d;default:var f=null;if(2<arguments.length){for(var f=
0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lt.a"></a>[function <span class="apidocSignatureSpan">mori.lt.</span>a (a, b)](#apidoc.element.mori.lt.a)
- description and source-code
```javascript
a = function (a, b){return a<b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lt.b"></a>[function <span class="apidocSignatureSpan">mori.lt.</span>b ()](#apidoc.element.mori.lt.b)
- description and source-code
```javascript
b = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lt.d"></a>[function <span class="apidocSignatureSpan">mori.lt.</span>d (a, c, d)](#apidoc.element.mori.lt.d)
- description and source-code
```javascript
function b(a, c, d){for(;;)if(a<c)if(K(d))a=c,c=G(d),d=K(d);else return c<G(d);else return!1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lt.f"></a>[function <span class="apidocSignatureSpan">mori.lt.</span>f (a)](#apidoc.element.mori.lt.f)
- description and source-code
```javascript
f = function (a){var c=
G(a);a=K(a);var g=G(a);a=H(a);return b(c,g,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lt.f1"></a>[function <span class="apidocSignatureSpan">mori.lt.</span>f1 ()](#apidoc.element.mori.lt.f1)
- description and source-code
```javascript
f1 = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lt.f2"></a>[function <span class="apidocSignatureSpan">mori.lt.</span>f2 (a, b)](#apidoc.element.mori.lt.f2)
- description and source-code
```javascript
f2 = function (a, b){return a<b}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.lte"></a>[module mori.lte](#apidoc.module.mori.lte)

#### <a name="apidoc.element.mori.lte.lte"></a>[function <span class="apidocSignatureSpan">mori.</span>lte (a, d, e)](#apidoc.element.mori.lte.lte)
- description and source-code
```javascript
lte = function (a, d, e){switch(arguments.length){case 1:return!0;case 2:return a<=d;default:var f=null;if(2<arguments.length){for(var f
=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+
2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lte.a"></a>[function <span class="apidocSignatureSpan">mori.lte.</span>a (a, b)](#apidoc.element.mori.lte.a)
- description and source-code
```javascript
a = function (a, b){return a<=b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lte.b"></a>[function <span class="apidocSignatureSpan">mori.lte.</span>b ()](#apidoc.element.mori.lte.b)
- description and source-code
```javascript
b = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lte.d"></a>[function <span class="apidocSignatureSpan">mori.lte.</span>d (a, c, d)](#apidoc.element.mori.lte.d)
- description and source-code
```javascript
function b(a, c, d){for(;;)if(a<=c)if(K(d))a=c,c=G(d),d=K(d);else return c<=G(d);else return!1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lte.f"></a>[function <span class="apidocSignatureSpan">mori.lte.</span>f (a)](#apidoc.element.mori.lte.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var g=G(a);a=H(a);return b(c,g,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lte.f1"></a>[function <span class="apidocSignatureSpan">mori.lte.</span>f1 ()](#apidoc.element.mori.lte.f1)
- description and source-code
```javascript
f1 = function (){return!0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.lte.f2"></a>[function <span class="apidocSignatureSpan">mori.lte.</span>f2 (a, b)](#apidoc.element.mori.lte.f2)
- description and source-code
```javascript
f2 = function (a, b){return a<=b}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.map"></a>[module mori.map](#apidoc.module.mori.map)

#### <a name="apidoc.element.mori.map.map"></a>[function <span class="apidocSignatureSpan">mori.</span>map (e, h, l, m, p)](#apidoc.element.mori.map.map)
- description and source-code
```javascript
map = function (e, h, l, m, p){switch(arguments.length){case 1:return d.call(this,e);case 2:return c.call(this,e,h);case 3:return b.call(this
,e,h,l);case 4:return a.call(this,
e,h,l,m);default:var q=null;if(4<arguments.length){for(var q=0,s=Array(arguments.length-4);q<s.length;)s[q]=arguments[q+4],++q;q
=new F(s,0)}return f.d(e,h,l,m,q)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
You can use it from your projects like so:

'''javascript
var inc = function(n) {
  return n+1;
};

mori.intoArray(mori.map(inc, mori.vector(1,2,3,4,5)));
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
...
```

#### <a name="apidoc.element.mori.map.a"></a>[function <span class="apidocSignatureSpan">mori.map.</span>a (a, b)](#apidoc.element.mori.map.a)
- description and source-code
```javascript
function c(a, b){return new V(null,function(){var c=D(b);if(c){if(fd(c)){for(var d=Yb(c),f=Q(d),q=Td(f),s=0;;)if(s<f)Xd(q,function
(){var b=C.a(d,s);return a.b?a.b(b):a.call(null,b)}()),s+=1;else break;return Wd(q.ca(),e.a(a,Zb(c)))}return M(function(){var b=
G(c);return a.b?a.b(b):a.call(null,b)}(),e.a(a,H(c)))}return null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map.b"></a>[function <span class="apidocSignatureSpan">mori.map.</span>b (a)](#apidoc.element.mori.map.b)
- description and source-code
```javascript
function d(a){return function(b){return function(){function c(d,e){var f=a.b?a.b(e):a.call(null,e);return b.a?b.a(d,f):b.call(null
,d,f)}function d(a){return b.b?
b.b(a):b.call(null,a)}function e(){return b.l?b.l():b.call(null)}var f=null,s=function(){function c(a,b,e){var f=null;if(2<arguments
.length){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return d.call(this,a,b,f)}function
 d(c,e,f){e=T.c(a,e,f);return b.a?b.a(c,e):b.call(null,c,e)}c.i=2;c.f=function(a){var b=G(a);a=K(a);var c=G(a);a=H(a);return d(b
,c,a)};c.d=d;return c}(),f=function(a,b,f){switch(arguments.length){case 0:return e.call(this);case 1:return d.call(this,
a);case 2:return c.call(this,a,b);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)
h[g]=arguments[g+2],++g;g=new F(h,0)}return s.d(a,b,g)}throw Error("Invalid arity: "+arguments.length);};f.i=2;f.f=s.f;f.l=e;f.b
=d;f.a=c;f.d=s.d;return f}()}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map.c"></a>[function <span class="apidocSignatureSpan">mori.map.</span>c (a, b, c)](#apidoc.element.mori.map.c)
- description and source-code
```javascript
function b(a, b, c){return new V(null,function(){var d=D(b),f=D(c);if(d&&f){var q=M,s;s=G(d);var u=G(f);s=a.a?a.a(s,u):a.call(null
,s,u);d=q(s,e.c(a,H(d),H(f)))}else d=
null;return d},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map.d"></a>[function <span class="apidocSignatureSpan">mori.map.</span>d (a, c, d, f, g)](#apidoc.element.mori.map.d)
- description and source-code
```javascript
function b(a, c, d, f, g){var h=function y(a){return new V(null,function(){var b=e.a(D,a);return Ee(ud,b)?M(e.a(G,b),y(e.a(H,b))):null},null,null)};return
 e.a(function(){return function(b){return T.a(a,b)}}(h),h(Nc.d(g,f,Kc([d,c],0))))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map.f"></a>[function <span class="apidocSignatureSpan">mori.map.</span>f (a)](#apidoc.element.mori.map.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=K(a);var e=G(a);a=K(a);var f=G(a);a=H(a);return b(c,d,e,f,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map.f1"></a>[function <span class="apidocSignatureSpan">mori.map.</span>f1 (a)](#apidoc.element.mori.map.f1)
- description and source-code
```javascript
function d(a){return function(b){return function(){function c(d,e){var f=a.b?a.b(e):a.call(null,e);return b.a?b.a(d,f):b.call(null
,d,f)}function d(a){return b.b?
b.b(a):b.call(null,a)}function e(){return b.l?b.l():b.call(null)}var f=null,s=function(){function c(a,b,e){var f=null;if(2<arguments
.length){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return d.call(this,a,b,f)}function
 d(c,e,f){e=T.c(a,e,f);return b.a?b.a(c,e):b.call(null,c,e)}c.i=2;c.f=function(a){var b=G(a);a=K(a);var c=G(a);a=H(a);return d(b
,c,a)};c.d=d;return c}(),f=function(a,b,f){switch(arguments.length){case 0:return e.call(this);case 1:return d.call(this,
a);case 2:return c.call(this,a,b);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)
h[g]=arguments[g+2],++g;g=new F(h,0)}return s.d(a,b,g)}throw Error("Invalid arity: "+arguments.length);};f.i=2;f.f=s.f;f.l=e;f.b
=d;f.a=c;f.d=s.d;return f}()}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map.f2"></a>[function <span class="apidocSignatureSpan">mori.map.</span>f2 (a, b)](#apidoc.element.mori.map.f2)
- description and source-code
```javascript
function c(a, b){return new V(null,function(){var c=D(b);if(c){if(fd(c)){for(var d=Yb(c),f=Q(d),q=Td(f),s=0;;)if(s<f)Xd(q,function
(){var b=C.a(d,s);return a.b?a.b(b):a.call(null,b)}()),s+=1;else break;return Wd(q.ca(),e.a(a,Zb(c)))}return M(function(){var b=
G(c);return a.b?a.b(b):a.call(null,b)}(),e.a(a,H(c)))}return null},null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.map.f3"></a>[function <span class="apidocSignatureSpan">mori.map.</span>f3 (a, b, c)](#apidoc.element.mori.map.f3)
- description and source-code
```javascript
function b(a, b, c){return new V(null,function(){var d=D(b),f=D(c);if(d&&f){var q=M,s;s=G(d);var u=G(f);s=a.a?a.a(s,u):a.call(null
,s,u);d=q(s,e.c(a,H(d),H(f)))}else d=
null;return d},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map.f4"></a>[function <span class="apidocSignatureSpan">mori.map.</span>f4 (a, b, c, d)](#apidoc.element.mori.map.f4)
- description and source-code
```javascript
function a(a, b, c, d){return new V(null,function(){var f=D(b),q=D(c),s=D(d);if(f&&q&&s){var u=M,v;v=G(f);var y=G(q),B=G(s);v=a.c?a
.c(v,y,B):a.call(null,v,y,B);f=u(v,e.n(a,H(f),H(q),H(s)))}else f=null;return f},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.map.n"></a>[function <span class="apidocSignatureSpan">mori.map.</span>n (a, b, c, d)](#apidoc.element.mori.map.n)
- description and source-code
```javascript
function a(a, b, c, d){return new V(null,function(){var f=D(b),q=D(c),s=D(d);if(f&&q&&s){var u=M,v;v=G(f);var y=G(q),B=G(s);v=a.c?a
.c(v,y,B):a.call(null,v,y,B);f=u(v,e.n(a,H(f),H(q),H(s)))}else f=null;return f},null,null)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.mapcat"></a>[module mori.mapcat](#apidoc.module.mori.mapcat)

#### <a name="apidoc.element.mori.mapcat.mapcat"></a>[function <span class="apidocSignatureSpan">mori.</span>mapcat (b, e)](#apidoc.element.mori.mapcat.mapcat)
- description and source-code
```javascript
mapcat = function (b, e){switch(arguments.length){case 1:return a.call(this,b);default:var f=null;if(1<arguments.length){for(var f=0,g=Array
(arguments.length-1);f<g.length;)g[f]=arguments[f+1],++f;f=new F(g,0)}return c.d(b,f)}throw Error("Invalid arity: "+arguments.length
);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mapcat.b"></a>[function <span class="apidocSignatureSpan">mori.mapcat.</span>b (a)](#apidoc.element.mori.mapcat.b)
- description and source-code
```javascript
function a(a){return Ie.a(Oe.b(a),Ve)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mapcat.d"></a>[function <span class="apidocSignatureSpan">mori.mapcat.</span>d (a, c)](#apidoc.element.mori.mapcat.d)
- description and source-code
```javascript
function b(a, c){return T.a(ae,T.c(Oe,a,c))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mapcat.f"></a>[function <span class="apidocSignatureSpan">mori.mapcat.</span>f (a)](#apidoc.element.mori.mapcat.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=H(a);return b(c,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mapcat.f1"></a>[function <span class="apidocSignatureSpan">mori.mapcat.</span>f1 (a)](#apidoc.element.mori.mapcat.f1)
- description and source-code
```javascript
function a(a){return Ie.a(Oe.b(a),Ve)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.merge"></a>[module mori.merge](#apidoc.module.mori.merge)

#### <a name="apidoc.element.mori.merge.merge"></a>[function <span class="apidocSignatureSpan">mori.</span>merge (a)](#apidoc.element.mori.merge.merge)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.merge.d"></a>[function <span class="apidocSignatureSpan">mori.merge.</span>d (a)](#apidoc.element.mori.merge.d)
- description and source-code
```javascript
function b(a){return t(Fe(ud,a))?A.a(function(a,b){return Nc.a(t(a)?a:Uf,b)},a):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.merge.f"></a>[function <span class="apidocSignatureSpan">mori.merge.</span>f (a)](#apidoc.element.mori.merge.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.mergeWith"></a>[module mori.mergeWith](#apidoc.module.mori.mergeWith)

#### <a name="apidoc.element.mori.mergeWith.mergeWith"></a>[function <span class="apidocSignatureSpan">mori.</span>mergeWith (a, d)](#apidoc.element.mori.mergeWith.mergeWith)
- description and source-code
```javascript
function a(a, d){var e=null;if(1<arguments.length){for(var e=0,f=Array(arguments.length-1);e<f.length;)f[e]=arguments[e+1],++e;e=
new F(f,0)}return b.call(this,a,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mergeWith.d"></a>[function <span class="apidocSignatureSpan">mori.mergeWith.</span>d (a, b)](#apidoc.element.mori.mergeWith.d)
- description and source-code
```javascript
function b(a, b){return t(Fe(ud,b))?A.a(function(a){return function(b,c){return A.c(a,t(b)?b:Uf,D(c))}}(function(b,d){var g=G(d),h=Lc(d);return
 nd(b,g)?Rc.c(b,g,function(){var d=S.a(b,g);return a.a?a.a(d,h):a.call(null,d,h)}()):Rc.c(b,g,h)}),b):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mergeWith.f"></a>[function <span class="apidocSignatureSpan">mori.mergeWith.</span>f (a)](#apidoc.element.mori.mergeWith.f)
- description and source-code
```javascript
f = function (a){var d=G(a);a=H(a);return b(d,a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.mutable"></a>[module mori.mutable](#apidoc.module.mori.mutable)

#### <a name="apidoc.element.mori.mutable.assoc"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>assoc (a, d, e, f)](#apidoc.element.mori.mutable.assoc)
- description and source-code
```javascript
assoc = function (a, d, e, f){switch(arguments.length){case 3:return Rb(a,d,e);default:var g=null;if(3<arguments.length){for(var g=0,h=Array
(arguments.length-3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return b.d(a,d,e,g)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.conj"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>conj (b, e, f)](#apidoc.element.mori.mutable.conj)
- description and source-code
```javascript
conj = function (b, e, f){switch(arguments.length){case 0:return a.call(this);case 1:return b;case 2:return Pb(b,
e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F
(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
var v2 = mori.conj(v1, 4);
v1.toString(); // => '[1 2 3]'
v2.toString(); // => '[1 2 3 4]'
'''

'''javascript
var sum = function(a, b) {
return a + b;
...
```

#### <a name="apidoc.element.mori.mutable.disj"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>disj (a, d, e)](#apidoc.element.mori.mutable.disj)
- description and source-code
```javascript
disj = function (a, d, e){switch(arguments.length){case 2:return Vb(a,d);default:var f=null;if(2<arguments.length){for(var f=0,g=Array(arguments
.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.dissoc"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>dissoc (a, d, e)](#apidoc.element.mori.mutable.dissoc)
- description and source-code
```javascript
dissoc = function (a, d, e){switch(arguments.length){case 2:return Sb(a,d);default:var f=null;if(2<
arguments.length){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw
 Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.freeze"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>freeze (a)](#apidoc.element.mori.mutable.freeze)
- description and source-code
```javascript
function ce(a){return Qb(a)}
```
- example usage
```shell
...
// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''

### ES6 Map/Set inspired interfaces
...
```

#### <a name="apidoc.element.mori.mutable.pop"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>pop (a)](#apidoc.element.mori.mutable.pop)
- description and source-code
```javascript
pop = function (a){return Ub(a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.thaw"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>thaw (a)](#apidoc.element.mori.mutable.thaw)
- description and source-code
```javascript
thaw = function (a){return Ob(a)}
```
- example usage
```shell
...
  print("Array push " + arr.length + " items " + ((new Date())-s));
  gc();
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
...
```



# <a name="apidoc.module.mori.mutable.assoc"></a>[module mori.mutable.assoc](#apidoc.module.mori.mutable.assoc)

#### <a name="apidoc.element.mori.mutable.assoc.assoc"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>assoc (a, d, e, f)](#apidoc.element.mori.mutable.assoc.assoc)
- description and source-code
```javascript
assoc = function (a, d, e, f){switch(arguments.length){case 3:return Rb(a,d,e);default:var g=null;if(3<arguments.length){for(var g=0,h=Array
(arguments.length-3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return b.d(a,d,e,g)}throw Error("Invalid arity: "+arguments
.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.assoc.c"></a>[function <span class="apidocSignatureSpan">mori.mutable.assoc.</span>c (a, b, e)](#apidoc.element.mori.mutable.assoc.c)
- description and source-code
```javascript
c = function (a, b, e){return Rb(a,b,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.assoc.d"></a>[function <span class="apidocSignatureSpan">mori.mutable.assoc.</span>d (a, c, d, h)](#apidoc.element.mori.mutable.assoc.d)
- description and source-code
```javascript
function b(a, c, d, h){for(;;)if(a=Rb(a,c,d),t(h))c=G(h),d=Lc(h),h=K(K(h));else return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.assoc.f"></a>[function <span class="apidocSignatureSpan">mori.mutable.assoc.</span>f (a)](#apidoc.element.mori.mutable.assoc.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var g=G(a);a=K(a);var h=G(a);a=H(a);return b(c,g,h,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.assoc.f3"></a>[function <span class="apidocSignatureSpan">mori.mutable.assoc.</span>f3 (a, b, e)](#apidoc.element.mori.mutable.assoc.f3)
- description and source-code
```javascript
f3 = function (a, b, e){return Rb(a,b,e)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.mutable.conj"></a>[module mori.mutable.conj](#apidoc.module.mori.mutable.conj)

#### <a name="apidoc.element.mori.mutable.conj.conj"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>conj (b, e, f)](#apidoc.element.mori.mutable.conj.conj)
- description and source-code
```javascript
conj = function (b, e, f){switch(arguments.length){case 0:return a.call(this);case 1:return b;case 2:return Pb(b,
e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F
(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
var v2 = mori.conj(v1, 4);
v1.toString(); // => '[1 2 3]'
v2.toString(); // => '[1 2 3 4]'
'''

'''javascript
var sum = function(a, b) {
return a + b;
...
```

#### <a name="apidoc.element.mori.mutable.conj.a"></a>[function <span class="apidocSignatureSpan">mori.mutable.conj.</span>a (a, b)](#apidoc.element.mori.mutable.conj.a)
- description and source-code
```javascript
a = function (a, b){return Pb(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.conj.b"></a>[function <span class="apidocSignatureSpan">mori.mutable.conj.</span>b (a)](#apidoc.element.mori.mutable.conj.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.conj.d"></a>[function <span class="apidocSignatureSpan">mori.mutable.conj.</span>d (a, c, d)](#apidoc.element.mori.mutable.conj.d)
- description and source-code
```javascript
function b(a, c, d){for(;;)if(a=Pb(a,c),t(d))c=G(d),d=K(d);else return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.conj.f"></a>[function <span class="apidocSignatureSpan">mori.mutable.conj.</span>f (a)](#apidoc.element.mori.mutable.conj.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=H(a);return b(c,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.conj.f0"></a>[function <span class="apidocSignatureSpan">mori.mutable.conj.</span>f0 ()](#apidoc.element.mori.mutable.conj.f0)
- description and source-code
```javascript
function a(){return Ob(Mc)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.conj.f1"></a>[function <span class="apidocSignatureSpan">mori.mutable.conj.</span>f1 (a)](#apidoc.element.mori.mutable.conj.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.conj.f2"></a>[function <span class="apidocSignatureSpan">mori.mutable.conj.</span>f2 (a, b)](#apidoc.element.mori.mutable.conj.f2)
- description and source-code
```javascript
f2 = function (a, b){return Pb(a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.mutable.conj.l"></a>[function <span class="apidocSignatureSpan">mori.mutable.conj.</span>l ()](#apidoc.element.mori.mutable.conj.l)
- description and source-code
```javascript
function a(){return Ob(Mc)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.mutable.disj"></a>[module mori.mutable.disj](#apidoc.module.mori.mutable.disj)

#### <a name="apidoc.element.mori.mutable.disj.disj"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>disj (a, d, e)](#apidoc.element.mori.mutable.disj.disj)
- description and source-code
```javascript
disj = function (a, d, e){switch(arguments.length){case 2:return Vb(a,d);default:var f=null;if(2<arguments.length){for(var f=0,g=Array(arguments
.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.disj.a"></a>[function <span class="apidocSignatureSpan">mori.mutable.disj.</span>a (a, b)](#apidoc.element.mori.mutable.disj.a)
- description and source-code
```javascript
a = function (a, b){return Vb(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.disj.d"></a>[function <span class="apidocSignatureSpan">mori.mutable.disj.</span>d (a, c, d)](#apidoc.element.mori.mutable.disj.d)
- description and source-code
```javascript
function b(a, c, d){for(;;)if(a=Vb(a,c),t(d))c=G(d),d=K(d);
else return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.disj.f"></a>[function <span class="apidocSignatureSpan">mori.mutable.disj.</span>f (a)](#apidoc.element.mori.mutable.disj.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var g=G(a);a=H(a);return b(c,g,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.disj.f2"></a>[function <span class="apidocSignatureSpan">mori.mutable.disj.</span>f2 (a, b)](#apidoc.element.mori.mutable.disj.f2)
- description and source-code
```javascript
f2 = function (a, b){return Vb(a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.mutable.dissoc"></a>[module mori.mutable.dissoc](#apidoc.module.mori.mutable.dissoc)

#### <a name="apidoc.element.mori.mutable.dissoc.dissoc"></a>[function <span class="apidocSignatureSpan">mori.mutable.</span>dissoc (a, d, e)](#apidoc.element.mori.mutable.dissoc.dissoc)
- description and source-code
```javascript
dissoc = function (a, d, e){switch(arguments.length){case 2:return Sb(a,d);default:var f=null;if(2<
arguments.length){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,0)}return b.d(a,d,f)}throw
 Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.dissoc.a"></a>[function <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>a (a, b)](#apidoc.element.mori.mutable.dissoc.a)
- description and source-code
```javascript
a = function (a, b){return Sb(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.dissoc.d"></a>[function <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>d (a, c, d)](#apidoc.element.mori.mutable.dissoc.d)
- description and source-code
```javascript
function b(a, c, d){for(;;)if(a=Sb(a,c),t(d))c=G(d),d=K(d);else return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.dissoc.f"></a>[function <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>f (a)](#apidoc.element.mori.mutable.dissoc.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var g=G(a);a=H(a);return b(c,g,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.mutable.dissoc.f2"></a>[function <span class="apidocSignatureSpan">mori.mutable.dissoc.</span>f2 (a, b)](#apidoc.element.mori.mutable.dissoc.f2)
- description and source-code
```javascript
f2 = function (a, b){return Sb(a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.notEquals"></a>[module mori.notEquals](#apidoc.module.mori.notEquals)

#### <a name="apidoc.element.mori.notEquals.notEquals"></a>[function <span class="apidocSignatureSpan">mori.</span>notEquals (b, e, f)](#apidoc.element.mori.notEquals.notEquals)
- description and source-code
```javascript
notEquals = function (b, e, f){switch(arguments.length){case 1:return!1;case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length
){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid
 arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.notEquals.a"></a>[function <span class="apidocSignatureSpan">mori.notEquals.</span>a (a, b)](#apidoc.element.mori.notEquals.a)
- description and source-code
```javascript
function a(a, b){return!sc.a(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.notEquals.b"></a>[function <span class="apidocSignatureSpan">mori.notEquals.</span>b ()](#apidoc.element.mori.notEquals.b)
- description and source-code
```javascript
b = function (){return!1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.notEquals.d"></a>[function <span class="apidocSignatureSpan">mori.notEquals.</span>d (a, c, d)](#apidoc.element.mori.notEquals.d)
- description and source-code
```javascript
function b(a, c, d){return Aa(T.n(sc,a,c,d))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.notEquals.f"></a>[function <span class="apidocSignatureSpan">mori.notEquals.</span>f (a)](#apidoc.element.mori.notEquals.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=H(a);return b(c,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.notEquals.f1"></a>[function <span class="apidocSignatureSpan">mori.notEquals.</span>f1 ()](#apidoc.element.mori.notEquals.f1)
- description and source-code
```javascript
f1 = function (){return!1}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.notEquals.f2"></a>[function <span class="apidocSignatureSpan">mori.notEquals.</span>f2 (a, b)](#apidoc.element.mori.notEquals.f2)
- description and source-code
```javascript
function a(a, b){return!sc.a(a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.nth"></a>[module mori.nth](#apidoc.module.mori.nth)

#### <a name="apidoc.element.mori.nth.nth"></a>[function <span class="apidocSignatureSpan">mori.</span>nth (c, e, f)](#apidoc.element.mori.nth.nth)
- description and source-code
```javascript
nth = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.nth.a"></a>[function <span class="apidocSignatureSpan">mori.nth.</span>a (a, b)](#apidoc.element.mori.nth.a)
- description and source-code
```javascript
function b(a, b){if("number"!==
typeof b)throw Error("index argument to nth must be a number");if(null==a)return a;if(a&&(a.j&16||a.Qb))return a.Q(null,b);if(a
instanceof Array||"string"===typeof a)return b<a.length?a[b]:null;if(w(Ta,a))return C.a(a,b);if(a?a.j&64||a.jb||(a.j?0:w(Ua,a)):
w(Ua,a))return Pc.a(a,b);throw Error([z("nth not supported on this type "),z(Da(Ba(a)))].join(""));}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.nth.c"></a>[function <span class="apidocSignatureSpan">mori.nth.</span>c (a, b, c)](#apidoc.element.mori.nth.c)
- description and source-code
```javascript
function a(a, b, c){if("number"!==typeof b)throw Error("index argument to nth must be a number.");if(null==a)return c;if(a&&(a.j&16
||a.Qb))return a.$(null,b,c);if(a instanceof Array||"string"===typeof a)return b<a.length?a[b]:c;if(w(Ta,a))return C.a(a,b);if(a
?a.j&64||a.jb||(a.j?0:w(Ua,a)):w(Ua,a))return Pc.c(a,b,c);throw Error([z("nth not supported on this type "),z(Da(Ba(a)))].join(""));}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.nth.f2"></a>[function <span class="apidocSignatureSpan">mori.nth.</span>f2 (a, b)](#apidoc.element.mori.nth.f2)
- description and source-code
```javascript
function b(a, b){if("number"!==
typeof b)throw Error("index argument to nth must be a number");if(null==a)return a;if(a&&(a.j&16||a.Qb))return a.Q(null,b);if(a
instanceof Array||"string"===typeof a)return b<a.length?a[b]:null;if(w(Ta,a))return C.a(a,b);if(a?a.j&64||a.jb||(a.j?0:w(Ua,a)):
w(Ua,a))return Pc.a(a,b);throw Error([z("nth not supported on this type "),z(Da(Ba(a)))].join(""));}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.nth.f3"></a>[function <span class="apidocSignatureSpan">mori.nth.</span>f3 (a, b, c)](#apidoc.element.mori.nth.f3)
- description and source-code
```javascript
function a(a, b, c){if("number"!==typeof b)throw Error("index argument to nth must be a number.");if(null==a)return c;if(a&&(a.j&16
||a.Qb))return a.$(null,b,c);if(a instanceof Array||"string"===typeof a)return b<a.length?a[b]:c;if(w(Ta,a))return C.a(a,b);if(a
?a.j&64||a.jb||(a.j?0:w(Ua,a)):w(Ua,a))return Pc.c(a,b,c);throw Error([z("nth not supported on this type "),z(Da(Ba(a)))].join(""));}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.partial"></a>[module mori.partial](#apidoc.module.mori.partial)

#### <a name="apidoc.element.mori.partial.partial"></a>[function <span class="apidocSignatureSpan">mori.</span>partial (d, g, h, l, m)](#apidoc.element.mori.partial.partial)
- description and source-code
```javascript
partial = function (d, g, h, l, m){switch(arguments.length){case 1:return d;case 2:return c.call(this,d,g);case 3:return b.call(this,d,g,h);case
 4:return a.call(this,d,g,h,l);default:var p=null;if(4<arguments.length){for(var p=
0,q=Array(arguments.length-4);p<q.length;)q[p]=arguments[p+4],++p;p=new F(q,0)}return e.d(d,g,h,l,p)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.a"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>a (a, b)](#apidoc.element.mori.partial.a)
- description and source-code
```javascript
function c(a, b){return function(){function c(d,e,h){return a.n?a.n(b,d,e,h):a.call(null,b,d,e,h)}function d(c,e){return a.c?a.c(
b,c,e):a.call(null,b,c,e)}function e(c){return a.a?a.a(b,c):a.call(null,b,c)}function p(){return a.b?a.b(b):a.call(null,b)}var q
=null,s=function(){function c(a,b,e,f){var g=null;if(3<arguments.length){for(var g=0,
h=Array(arguments.length-3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return d.call(this,a,b,e,g)}function d(c,e,h,l){return
 T.d(a,b,c,e,h,Kc([l],0))}c.i=3;c.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var e=G(a);a=H(a);return d(b,c,e,a)};c.d=d;return
 c}(),q=function(a,b,f,g){switch(arguments.length){case 0:return p.call(this);case 1:return e.call(this,a);case 2:return d.call(
this,a,b);case 3:return c.call(this,a,b,f);default:var q=null;if(3<arguments.length){for(var q=0,N=Array(arguments.length-
3);q<N.length;)N[q]=arguments[q+3],++q;q=new F(N,0)}return s.d(a,b,f,q)}throw Error("Invalid arity: "+arguments.length);};q.i=3;
q.f=s.f;q.l=p;q.b=e;q.a=d;q.c=c;q.d=s.d;return q}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.b"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>b (a)](#apidoc.element.mori.partial.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.c"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>c (a, b, c)](#apidoc.element.mori.partial.c)
- description and source-code
```javascript
function b(a, b, c){return function(){function d(e,l,m){return a.r?a.r(b,c,e,l,m):a.call(null,b,c,e,l,m)}function e(d,l){return a.
n?a.n(b,c,d,l):a.call(null,b,c,d,l)}function p(d){return a.c?a.c(b,c,d):a.call(null,b,c,d)}function q(){return a.a?a.a(b,c):a.call
(null,b,c)}var s=null,u=function(){function d(a,b,c,f){var g=null;if(3<arguments.length){for(var g=0,h=Array(arguments.length-
3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return e.call(this,a,b,c,g)}function e(d,l,m,p){return T.d(a,b,c,d,l,Kc([m,p
],0))}d.i=3;d.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return e(b,c,d,a)};d.d=e;return d}(),s=function
(a,b,c,f){switch(arguments.length){case 0:return q.call(this);case 1:return p.call(this,a);case 2:return e.call(this,a,b);case 3
:return d.call(this,a,b,c);default:var g=null;if(3<arguments.length){for(var g=0,h=Array(arguments.length-3);g<h.length;)h[g]=
arguments[g+3],++g;g=new F(h,0)}return u.d(a,b,c,g)}throw Error("Invalid arity: "+arguments.length);};s.i=3;s.f=u.f;s.l=q;s.b=p;
s.a=e;s.c=d;s.d=u.d;return s}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.d"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>d (a, c, d, e, f)](#apidoc.element.mori.partial.d)
- description and source-code
```javascript
function b(a, c, d, e, f){return function(){function b(a){var c=null;if(0<arguments.length){for(var c=0,d=Array(arguments.length-
0);c<d.length;)d[c]=arguments[c+0],++c;c=new F(d,0)}return g.call(this,c)}function g(b){return T.r(a,c,d,e,ae.a(f,b))}b.i=0;b.f=
function(a){a=D(a);return g(a)};b.d=g;return b}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.f"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>f (a)](#apidoc.element.mori.partial.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=K(a);var e=G(a);a=K(a);var f=G(a);a=H(a);return b(c,d,e,f,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.f1"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>f1 (a)](#apidoc.element.mori.partial.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.f2"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>f2 (a, b)](#apidoc.element.mori.partial.f2)
- description and source-code
```javascript
function c(a, b){return function(){function c(d,e,h){return a.n?a.n(b,d,e,h):a.call(null,b,d,e,h)}function d(c,e){return a.c?a.c(
b,c,e):a.call(null,b,c,e)}function e(c){return a.a?a.a(b,c):a.call(null,b,c)}function p(){return a.b?a.b(b):a.call(null,b)}var q
=null,s=function(){function c(a,b,e,f){var g=null;if(3<arguments.length){for(var g=0,
h=Array(arguments.length-3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return d.call(this,a,b,e,g)}function d(c,e,h,l){return
 T.d(a,b,c,e,h,Kc([l],0))}c.i=3;c.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var e=G(a);a=H(a);return d(b,c,e,a)};c.d=d;return
 c}(),q=function(a,b,f,g){switch(arguments.length){case 0:return p.call(this);case 1:return e.call(this,a);case 2:return d.call(
this,a,b);case 3:return c.call(this,a,b,f);default:var q=null;if(3<arguments.length){for(var q=0,N=Array(arguments.length-
3);q<N.length;)N[q]=arguments[q+3],++q;q=new F(N,0)}return s.d(a,b,f,q)}throw Error("Invalid arity: "+arguments.length);};q.i=3;
q.f=s.f;q.l=p;q.b=e;q.a=d;q.c=c;q.d=s.d;return q}()}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.partial.f3"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>f3 (a, b, c)](#apidoc.element.mori.partial.f3)
- description and source-code
```javascript
function b(a, b, c){return function(){function d(e,l,m){return a.r?a.r(b,c,e,l,m):a.call(null,b,c,e,l,m)}function e(d,l){return a.
n?a.n(b,c,d,l):a.call(null,b,c,d,l)}function p(d){return a.c?a.c(b,c,d):a.call(null,b,c,d)}function q(){return a.a?a.a(b,c):a.call
(null,b,c)}var s=null,u=function(){function d(a,b,c,f){var g=null;if(3<arguments.length){for(var g=0,h=Array(arguments.length-
3);g<h.length;)h[g]=arguments[g+3],++g;g=new F(h,0)}return e.call(this,a,b,c,g)}function e(d,l,m,p){return T.d(a,b,c,d,l,Kc([m,p
],0))}d.i=3;d.f=function(a){var b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return e(b,c,d,a)};d.d=e;return d}(),s=function
(a,b,c,f){switch(arguments.length){case 0:return q.call(this);case 1:return p.call(this,a);case 2:return e.call(this,a,b);case 3
:return d.call(this,a,b,c);default:var g=null;if(3<arguments.length){for(var g=0,h=Array(arguments.length-3);g<h.length;)h[g]=
arguments[g+3],++g;g=new F(h,0)}return u.d(a,b,c,g)}throw Error("Invalid arity: "+arguments.length);};s.i=3;s.f=u.f;s.l=q;s.b=p;
s.a=e;s.c=d;s.d=u.d;return s}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.f4"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>f4 (a, b, c, d)](#apidoc.element.mori.partial.f4)
- description and source-code
```javascript
function a(a, b, c, d){return function(){function e(m,p,q){return a.P?a.P(b,c,d,m,p,q):a.call(null,b,c,d,m,p,q)}function p(e,m){return
 a.r?a.r(b,c,d,e,m):a.call(null,b,c,d,e,m)}function q(e){return a.n?a.n(b,c,d,e):a.call(null,b,c,d,e)}function s(){return a.c?a.
c(b,c,d):a.call(null,b,c,d)}var u=null,v=function(){function e(a,b,c,d){var f=null;if(3<arguments.length){for(var f=0,g=Array(arguments
.length-3);f<g.length;)g[f]=arguments[f+
3],++f;f=new F(g,0)}return m.call(this,a,b,c,f)}function m(e,p,q,s){return T.d(a,b,c,d,e,Kc([p,q,s],0))}e.i=3;e.f=function(a){var
 b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return m(b,c,d,a)};e.d=m;return e}(),u=function(a,b,c,d){switch(arguments.length
){case 0:return s.call(this);case 1:return q.call(this,a);case 2:return p.call(this,a,b);case 3:return e.call(this,a,b,c);default
:var f=null;if(3<arguments.length){for(var f=0,g=Array(arguments.length-3);f<g.length;)g[f]=arguments[f+3],++f;f=
new F(g,0)}return v.d(a,b,c,f)}throw Error("Invalid arity: "+arguments.length);};u.i=3;u.f=v.f;u.l=s;u.b=q;u.a=p;u.c=e;u.d=v.d;return
 u}()}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partial.n"></a>[function <span class="apidocSignatureSpan">mori.partial.</span>n (a, b, c, d)](#apidoc.element.mori.partial.n)
- description and source-code
```javascript
function a(a, b, c, d){return function(){function e(m,p,q){return a.P?a.P(b,c,d,m,p,q):a.call(null,b,c,d,m,p,q)}function p(e,m){return
 a.r?a.r(b,c,d,e,m):a.call(null,b,c,d,e,m)}function q(e){return a.n?a.n(b,c,d,e):a.call(null,b,c,d,e)}function s(){return a.c?a.
c(b,c,d):a.call(null,b,c,d)}var u=null,v=function(){function e(a,b,c,d){var f=null;if(3<arguments.length){for(var f=0,g=Array(arguments
.length-3);f<g.length;)g[f]=arguments[f+
3],++f;f=new F(g,0)}return m.call(this,a,b,c,f)}function m(e,p,q,s){return T.d(a,b,c,d,e,Kc([p,q,s],0))}e.i=3;e.f=function(a){var
 b=G(a);a=K(a);var c=G(a);a=K(a);var d=G(a);a=H(a);return m(b,c,d,a)};e.d=m;return e}(),u=function(a,b,c,d){switch(arguments.length
){case 0:return s.call(this);case 1:return q.call(this,a);case 2:return p.call(this,a,b);case 3:return e.call(this,a,b,c);default
:var f=null;if(3<arguments.length){for(var f=0,g=Array(arguments.length-3);f<g.length;)g[f]=arguments[f+3],++f;f=
new F(g,0)}return v.d(a,b,c,f)}throw Error("Invalid arity: "+arguments.length);};u.i=3;u.f=v.f;u.l=s;u.b=q;u.a=p;u.c=e;u.d=v.d;return
 u}()}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.partition"></a>[module mori.partition](#apidoc.module.mori.partition)

#### <a name="apidoc.element.mori.partition.partition"></a>[function <span class="apidocSignatureSpan">mori.</span>partition (d, f, g, h)](#apidoc.element.mori.partition.partition)
- description and source-code
```javascript
partition = function (d, f, g, h){switch(arguments.length){case 2:return c.call(this,d,f);case 3:return b.call(this,d,f,g);case 4:return a.call
(this,d,f,g,h)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partition.a"></a>[function <span class="apidocSignatureSpan">mori.partition.</span>a (a, b)](#apidoc.element.mori.partition.a)
- description and source-code
```javascript
function c(a, b){return d.c(a,a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partition.c"></a>[function <span class="apidocSignatureSpan">mori.partition.</span>c (a, b, c)](#apidoc.element.mori.partition.c)
- description and source-code
```javascript
function b(a, b, c){return new V(null,function(){var h=D(c);if(h){var l=Pe.a(a,h);return a===Q(l)?M(l,d.c(a,b,Qe.a(b,h))):null}return
 null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partition.f2"></a>[function <span class="apidocSignatureSpan">mori.partition.</span>f2 (a, b)](#apidoc.element.mori.partition.f2)
- description and source-code
```javascript
function c(a, b){return d.c(a,a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.partition.f3"></a>[function <span class="apidocSignatureSpan">mori.partition.</span>f3 (a, b, c)](#apidoc.element.mori.partition.f3)
- description and source-code
```javascript
function b(a, b, c){return new V(null,function(){var h=D(c);if(h){var l=Pe.a(a,h);return a===Q(l)?M(l,d.c(a,b,Qe.a(b,h))):null}return
 null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partition.f4"></a>[function <span class="apidocSignatureSpan">mori.partition.</span>f4 (a, b, c, h)](#apidoc.element.mori.partition.f4)
- description and source-code
```javascript
function a(a, b, c, h){return new V(null,function(){var l=D(h);if(l){var m=Pe.a(a,l);return a===
Q(m)?M(m,d.n(a,b,c,Qe.a(b,l))):Ra(J,Pe.a(a,ae.a(m,c)))}return null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partition.n"></a>[function <span class="apidocSignatureSpan">mori.partition.</span>n (a, b, c, h)](#apidoc.element.mori.partition.n)
- description and source-code
```javascript
function a(a, b, c, h){return new V(null,function(){var l=D(h);if(l){var m=Pe.a(a,l);return a===
Q(m)?M(m,d.n(a,b,c,Qe.a(b,l))):Ra(J,Pe.a(a,ae.a(m,c)))}return null},null,null)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.partitionAll"></a>[module mori.partitionAll](#apidoc.module.mori.partitionAll)

#### <a name="apidoc.element.mori.partitionAll.partitionAll"></a>[function <span class="apidocSignatureSpan">mori.</span>partitionAll (d, f, g)](#apidoc.element.mori.partitionAll.partitionAll)
- description and source-code
```javascript
partitionAll = function (d, f, g){switch(arguments.length){case 1:return c.call(this,d);case 2:return b.call(this,d,f);case 3:return a.call(this,
d,f,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionAll.a"></a>[function <span class="apidocSignatureSpan">mori.partitionAll.</span>a (a, b)](#apidoc.element.mori.partitionAll.a)
- description and source-code
```javascript
function b(a, b){return d.c(a,a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionAll.b"></a>[function <span class="apidocSignatureSpan">mori.partitionAll.</span>b (a)](#apidoc.element.mori.partitionAll.b)
- description and source-code
```javascript
function c(a){return function(b){return function(c){return function(){function d(h,l){c.add(l);if(a===c.size()){var m=zf(c.e);c.
clear();return b.a?b.a(h,m):b.call(null,h,m)}return h}function l(a){if(!t(0===c.e.length)){var d=zf(c.e);c.clear();a=Bc(b.a?b.a(
a,d):b.call(null,a,d))}return b.b?b.b(a):b.call(null,a)}function m(){return b.l?
b.l():b.call(null)}var p=null,p=function(a,b){switch(arguments.length){case 0:return m.call(this);case 1:return l.call(this,a);case
 2:return d.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};p.l=m;p.b=l;p.a=d;return p}()}(new jh([]))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionAll.c"></a>[function <span class="apidocSignatureSpan">mori.partitionAll.</span>c (a, b, c)](#apidoc.element.mori.partitionAll.c)
- description and source-code
```javascript
function a(a, b, c){return new V(null,function(){var h=D(c);return h?M(Pe.a(a,h),d.c(a,b,Qe.a(b,h))):null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionAll.f1"></a>[function <span class="apidocSignatureSpan">mori.partitionAll.</span>f1 (a)](#apidoc.element.mori.partitionAll.f1)
- description and source-code
```javascript
function c(a){return function(b){return function(c){return function(){function d(h,l){c.add(l);if(a===c.size()){var m=zf(c.e);c.
clear();return b.a?b.a(h,m):b.call(null,h,m)}return h}function l(a){if(!t(0===c.e.length)){var d=zf(c.e);c.clear();a=Bc(b.a?b.a(
a,d):b.call(null,a,d))}return b.b?b.b(a):b.call(null,a)}function m(){return b.l?
b.l():b.call(null)}var p=null,p=function(a,b){switch(arguments.length){case 0:return m.call(this);case 1:return l.call(this,a);case
 2:return d.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};p.l=m;p.b=l;p.a=d;return p}()}(new jh([]))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionAll.f2"></a>[function <span class="apidocSignatureSpan">mori.partitionAll.</span>f2 (a, b)](#apidoc.element.mori.partitionAll.f2)
- description and source-code
```javascript
function b(a, b){return d.c(a,a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.partitionAll.f3"></a>[function <span class="apidocSignatureSpan">mori.partitionAll.</span>f3 (a, b, c)](#apidoc.element.mori.partitionAll.f3)
- description and source-code
```javascript
function a(a, b, c){return new V(null,function(){var h=D(c);return h?M(Pe.a(a,h),d.c(a,b,Qe.a(b,h))):null},null,null)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.partitionBy"></a>[module mori.partitionBy](#apidoc.module.mori.partitionBy)

#### <a name="apidoc.element.mori.partitionBy.partitionBy"></a>[function <span class="apidocSignatureSpan">mori.</span>partitionBy (c, e)](#apidoc.element.mori.partitionBy.partitionBy)
- description and source-code
```javascript
partitionBy = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionBy.a"></a>[function <span class="apidocSignatureSpan">mori.partitionBy.</span>a (a, b)](#apidoc.element.mori.partitionBy.a)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var f=D(b);if(f){var g=G(f),h=a.b?a.b(g):a.call(null,g),g=M(g,lh.a(function(b,c){return
 function(b){return sc.a(c,a.b?a.b(b):a.call(null,b))}}(g,h,f,f),K(f)));return M(g,c.a(a,D(Qe.a(Q(g),f))))}return null},null,
null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionBy.b"></a>[function <span class="apidocSignatureSpan">mori.partitionBy.</span>b (a)](#apidoc.element.mori.partitionBy.b)
- description and source-code
```javascript
function b(a){return function(b){return function(c,g){return function(){function h(h,l){var m=L.b?L.b(g):L.call(null,g),p=a.b?a.
b(l):a.call(null,l);ac(g,p);if(Nd(m,sh)||sc.a(p,m))return c.add(l),h;m=zf(c.e);c.clear();m=b.a?b.a(h,m):b.call(null,h,m);Ac(m)||
c.add(l);return m}function l(a){if(!t(0===c.e.length)){var d=zf(c.e);c.clear();a=Bc(b.a?b.a(a,d):b.call(null,a,d))}return b.b?b.
b(a):b.call(null,a)}function m(){return b.l?b.l():b.call(null)}var p=null,p=function(a,b){switch(arguments.length){case 0:return
 m.call(this);
case 1:return l.call(this,a);case 2:return h.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};p.l=m;p.b=l;p.a=h;
return p}()}(new jh([]),new Me(sh))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionBy.f1"></a>[function <span class="apidocSignatureSpan">mori.partitionBy.</span>f1 (a)](#apidoc.element.mori.partitionBy.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(c,g){return function(){function h(h,l){var m=L.b?L.b(g):L.call(null,g),p=a.b?a.
b(l):a.call(null,l);ac(g,p);if(Nd(m,sh)||sc.a(p,m))return c.add(l),h;m=zf(c.e);c.clear();m=b.a?b.a(h,m):b.call(null,h,m);Ac(m)||
c.add(l);return m}function l(a){if(!t(0===c.e.length)){var d=zf(c.e);c.clear();a=Bc(b.a?b.a(a,d):b.call(null,a,d))}return b.b?b.
b(a):b.call(null,a)}function m(){return b.l?b.l():b.call(null)}var p=null,p=function(a,b){switch(arguments.length){case 0:return
 m.call(this);
case 1:return l.call(this,a);case 2:return h.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};p.l=m;p.b=l;p.a=h;
return p}()}(new jh([]),new Me(sh))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.partitionBy.f2"></a>[function <span class="apidocSignatureSpan">mori.partitionBy.</span>f2 (a, b)](#apidoc.element.mori.partitionBy.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var f=D(b);if(f){var g=G(f),h=a.b?a.b(g):a.call(null,g),g=M(g,lh.a(function(b,c){return
 function(b){return sc.a(c,a.b?a.b(b):a.call(null,b))}}(g,h,f,f),K(f)));return M(g,c.a(a,D(Qe.a(Q(g),f))))}return null},null,
null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.pipeline"></a>[module mori.pipeline](#apidoc.module.mori.pipeline)

#### <a name="apidoc.element.mori.pipeline.pipeline"></a>[function <span class="apidocSignatureSpan">mori.</span>pipeline (a)](#apidoc.element.mori.pipeline.pipeline)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.pipeline.d"></a>[function <span class="apidocSignatureSpan">mori.pipeline.</span>d (a)](#apidoc.element.mori.pipeline.d)
- description and source-code
```javascript
function b(a){function b(a,c){return c.b?c.b(a):c.call(null,a)}return A.a?A.a(b,a):A.call(null,b,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.pipeline.f"></a>[function <span class="apidocSignatureSpan">mori.pipeline.</span>f (a)](#apidoc.element.mori.pipeline.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.primSeq"></a>[module mori.primSeq](#apidoc.module.mori.primSeq)

#### <a name="apidoc.element.mori.primSeq.primSeq"></a>[function <span class="apidocSignatureSpan">mori.</span>primSeq (c, e)](#apidoc.element.mori.primSeq.primSeq)
- description and source-code
```javascript
primSeq = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.primSeq.a"></a>[function <span class="apidocSignatureSpan">mori.primSeq.</span>a (a, b)](#apidoc.element.mori.primSeq.a)
- description and source-code
```javascript
function a(a, b){return b<a.length?new F(a,b):null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.primSeq.b"></a>[function <span class="apidocSignatureSpan">mori.primSeq.</span>b (a)](#apidoc.element.mori.primSeq.b)
- description and source-code
```javascript
function b(a){return c.a(a,0)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.primSeq.f1"></a>[function <span class="apidocSignatureSpan">mori.primSeq.</span>f1 (a)](#apidoc.element.mori.primSeq.f1)
- description and source-code
```javascript
function b(a){return c.a(a,0)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.primSeq.f2"></a>[function <span class="apidocSignatureSpan">mori.primSeq.</span>f2 (a, b)](#apidoc.element.mori.primSeq.f2)
- description and source-code
```javascript
function a(a, b){return b<a.length?new F(a,b):null}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.queue"></a>[module mori.queue](#apidoc.module.mori.queue)

#### <a name="apidoc.element.mori.queue.queue"></a>[function <span class="apidocSignatureSpan">mori.</span>queue (a)](#apidoc.element.mori.queue.queue)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.queue.d"></a>[function <span class="apidocSignatureSpan">mori.queue.</span>d (a)](#apidoc.element.mori.queue.d)
- description and source-code
```javascript
function b(a){return af.a?af.a(Mf,a):af.call(null,Mf,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.queue.f"></a>[function <span class="apidocSignatureSpan">mori.queue.</span>f (a)](#apidoc.element.mori.queue.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.range"></a>[module mori.range](#apidoc.module.mori.range)

#### <a name="apidoc.element.mori.range.range"></a>[function <span class="apidocSignatureSpan">mori.</span>range (e, g, h)](#apidoc.element.mori.range.range)
- description and source-code
```javascript
range = function (e, g, h){switch(arguments.length){case 0:return d.call(this);case 1:return c.call(this,e);case 2:return b.call(this,e,g);
case 3:return a.call(this,e,g,h)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.range.a"></a>[function <span class="apidocSignatureSpan">mori.range.</span>a (a, b)](#apidoc.element.mori.range.a)
- description and source-code
```javascript
function b(a, b){return e.c(a,b,1)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.range.b"></a>[function <span class="apidocSignatureSpan">mori.range.</span>b (a)](#apidoc.element.mori.range.b)
- description and source-code
```javascript
function c(a){return e.c(0,a,1)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.range.c"></a>[function <span class="apidocSignatureSpan">mori.range.</span>c (a, b, c)](#apidoc.element.mori.range.c)
- description and source-code
```javascript
function a(a, b, c){return new ph(null,a,b,c,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.range.f0"></a>[function <span class="apidocSignatureSpan">mori.range.</span>f0 ()](#apidoc.element.mori.range.f0)
- description and source-code
```javascript
function d(){return e.c(0,Number.MAX_VALUE,1)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.range.f1"></a>[function <span class="apidocSignatureSpan">mori.range.</span>f1 (a)](#apidoc.element.mori.range.f1)
- description and source-code
```javascript
function c(a){return e.c(0,a,1)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.range.f2"></a>[function <span class="apidocSignatureSpan">mori.range.</span>f2 (a, b)](#apidoc.element.mori.range.f2)
- description and source-code
```javascript
function b(a, b){return e.c(a,b,1)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.range.f3"></a>[function <span class="apidocSignatureSpan">mori.range.</span>f3 (a, b, c)](#apidoc.element.mori.range.f3)
- description and source-code
```javascript
function a(a, b, c){return new ph(null,a,b,c,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.range.l"></a>[function <span class="apidocSignatureSpan">mori.range.</span>l ()](#apidoc.element.mori.range.l)
- description and source-code
```javascript
function d(){return e.c(0,Number.MAX_VALUE,1)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.reduce"></a>[module mori.reduce](#apidoc.module.mori.reduce)

#### <a name="apidoc.element.mori.reduce.reduce"></a>[function <span class="apidocSignatureSpan">mori.</span>reduce (c, e, f)](#apidoc.element.mori.reduce.reduce)
- description and source-code
```javascript
reduce = function (c, e, f){switch(arguments.length){case 2:return b.call(this,
c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
...
v2.toString(); // => '[1 2 3 4]'
'''

'''javascript
var sum = function(a, b) {
  return a + b;
};
mori.reduce(sum, mori.vector(1, 2, 3, 4)); // => 10
'''

Lazy sequences!

'''javascript
var _ = mori;
_.intoArray(_.interpose("foo", _.vector(1, 2, 3, 4)));
...
```

#### <a name="apidoc.element.mori.reduce.a"></a>[function <span class="apidocSignatureSpan">mori.reduce.</span>a (a, b)](#apidoc.element.mori.reduce.a)
- description and source-code
```javascript
function b(a, b){return b&&(b.j&524288||b.Sb)?b.R(null,a):b instanceof Array?Dc.a(b,a):"string"===typeof b?Dc.a(b,a):w(vb,b)?wb.a
(b,a):P.a(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.reduce.c"></a>[function <span class="apidocSignatureSpan">mori.reduce.</span>c (a, b, c)](#apidoc.element.mori.reduce.c)
- description and source-code
```javascript
function a(a, b, c){return c&&(c.j&524288||c.Sb)?c.O(null,a,b):c instanceof Array?Dc.c(c,a,b):"string"===typeof c?Dc.c(c,a,b):w(vb
,c)?wb.c(c,a,b):P.c(a,b,c)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.reduce.f2"></a>[function <span class="apidocSignatureSpan">mori.reduce.</span>f2 (a, b)](#apidoc.element.mori.reduce.f2)
- description and source-code
```javascript
function b(a, b){return b&&(b.j&524288||b.Sb)?b.R(null,a):b instanceof Array?Dc.a(b,a):"string"===typeof b?Dc.a(b,a):w(vb,b)?wb.a
(b,a):P.a(a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.reduce.f3"></a>[function <span class="apidocSignatureSpan">mori.reduce.</span>f3 (a, b, c)](#apidoc.element.mori.reduce.f3)
- description and source-code
```javascript
function a(a, b, c){return c&&(c.j&524288||c.Sb)?c.O(null,a,b):c instanceof Array?Dc.c(c,a,b):"string"===typeof c?Dc.c(c,a,b):w(vb
,c)?wb.c(c,a,b):P.c(a,b,c)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.remove"></a>[module mori.remove](#apidoc.module.mori.remove)

#### <a name="apidoc.element.mori.remove.remove"></a>[function <span class="apidocSignatureSpan">mori.</span>remove (c, e)](#apidoc.element.mori.remove.remove)
- description and source-code
```javascript
remove = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.remove.a"></a>[function <span class="apidocSignatureSpan">mori.remove.</span>a (a, b)](#apidoc.element.mori.remove.a)
- description and source-code
```javascript
function a(a, b){return Xe.a(He(a),b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.remove.b"></a>[function <span class="apidocSignatureSpan">mori.remove.</span>b (a)](#apidoc.element.mori.remove.b)
- description and source-code
```javascript
function b(a){return Xe.b(He(a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.remove.f1"></a>[function <span class="apidocSignatureSpan">mori.remove.</span>f1 (a)](#apidoc.element.mori.remove.f1)
- description and source-code
```javascript
function b(a){return Xe.b(He(a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.remove.f2"></a>[function <span class="apidocSignatureSpan">mori.remove.</span>f2 (a, b)](#apidoc.element.mori.remove.f2)
- description and source-code
```javascript
function a(a, b){return Xe.a(He(a),b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.repeat"></a>[module mori.repeat](#apidoc.module.mori.repeat)

#### <a name="apidoc.element.mori.repeat.repeat"></a>[function <span class="apidocSignatureSpan">mori.</span>repeat (c, e)](#apidoc.element.mori.repeat.repeat)
- description and source-code
```javascript
repeat = function (c, e){switch(arguments.length){case 1:return b.call(this,
c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeat.a"></a>[function <span class="apidocSignatureSpan">mori.repeat.</span>a (a, b)](#apidoc.element.mori.repeat.a)
- description and source-code
```javascript
function a(a, b){return Pe.a(a,c.b(b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeat.b"></a>[function <span class="apidocSignatureSpan">mori.repeat.</span>b (a)](#apidoc.element.mori.repeat.b)
- description and source-code
```javascript
function b(a){return new V(null,function(){return M(a,c.b(a))},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeat.f1"></a>[function <span class="apidocSignatureSpan">mori.repeat.</span>f1 (a)](#apidoc.element.mori.repeat.f1)
- description and source-code
```javascript
function b(a){return new V(null,function(){return M(a,c.b(a))},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeat.f2"></a>[function <span class="apidocSignatureSpan">mori.repeat.</span>f2 (a, b)](#apidoc.element.mori.repeat.f2)
- description and source-code
```javascript
function a(a, b){return Pe.a(a,c.b(b))}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.repeatedly"></a>[module mori.repeatedly](#apidoc.module.mori.repeatedly)

#### <a name="apidoc.element.mori.repeatedly.repeatedly"></a>[function <span class="apidocSignatureSpan">mori.</span>repeatedly (c, e)](#apidoc.element.mori.repeatedly.repeatedly)
- description and source-code
```javascript
repeatedly = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeatedly.a"></a>[function <span class="apidocSignatureSpan">mori.repeatedly.</span>a (a, b)](#apidoc.element.mori.repeatedly.a)
- description and source-code
```javascript
function a(a, b){return Pe.a(a,c.b(b))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeatedly.b"></a>[function <span class="apidocSignatureSpan">mori.repeatedly.</span>b (a)](#apidoc.element.mori.repeatedly.b)
- description and source-code
```javascript
function b(a){return new V(null,function(){return M(a.l?a.l():a.call(null),c.b(a))},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeatedly.f1"></a>[function <span class="apidocSignatureSpan">mori.repeatedly.</span>f1 (a)](#apidoc.element.mori.repeatedly.f1)
- description and source-code
```javascript
function b(a){return new V(null,function(){return M(a.l?a.l():a.call(null),c.b(a))},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.repeatedly.f2"></a>[function <span class="apidocSignatureSpan">mori.repeatedly.</span>f2 (a, b)](#apidoc.element.mori.repeatedly.f2)
- description and source-code
```javascript
function a(a, b){return Pe.a(a,c.b(b))}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.sequence"></a>[module mori.sequence](#apidoc.module.mori.sequence)

#### <a name="apidoc.element.mori.sequence.sequence"></a>[function <span class="apidocSignatureSpan">mori.</span>sequence (b, e, f)](#apidoc.element.mori.sequence.sequence)
- description and source-code
```javascript
sequence = function (b, e, f){switch(arguments.length){case 1:return a.call(this,b);case 2:return new ze(ye(b,we(e)),null,null,null);default:
var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g]=arguments[g+2],++g;g=new F(h,0)}return
 c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sequence.a"></a>[function <span class="apidocSignatureSpan">mori.sequence.</span>a (a, b)](#apidoc.element.mori.sequence.a)
- description and source-code
```javascript
a = function (a, b){return new ze(ye(a,
we(b)),null,null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sequence.b"></a>[function <span class="apidocSignatureSpan">mori.sequence.</span>b (a)](#apidoc.element.mori.sequence.b)
- description and source-code
```javascript
function a(a){return kd(a)?a:(a=D(a))?a:J}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sequence.d"></a>[function <span class="apidocSignatureSpan">mori.sequence.</span>d (a, c, d)](#apidoc.element.mori.sequence.d)
- description and source-code
```javascript
function b(a, c, d){d=rd(M(c,d));c=[];d=D(d);for(var e=null,m=0,p=0;;)if(p<m){var q=e.Q(null,p);c.push(we(q));p+=1}else if(d=D(d))
e=d,fd(e)?(d=Yb(e),p=Zb(e),e=d,m=Q(d),d=p):(d=G(e),c.push(we(d)),d=K(e),e=null,m=0),p=0;else break;return new ze(Be.c(a,c,
Array(c.length)),null,null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sequence.f"></a>[function <span class="apidocSignatureSpan">mori.sequence.</span>f (a)](#apidoc.element.mori.sequence.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=H(a);return b(c,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sequence.f1"></a>[function <span class="apidocSignatureSpan">mori.sequence.</span>f1 (a)](#apidoc.element.mori.sequence.f1)
- description and source-code
```javascript
function a(a){return kd(a)?a:(a=D(a))?a:J}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sequence.f2"></a>[function <span class="apidocSignatureSpan">mori.sequence.</span>f2 (a, b)](#apidoc.element.mori.sequence.f2)
- description and source-code
```javascript
f2 = function (a, b){return new ze(ye(a,
we(b)),null,null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.sort"></a>[module mori.sort](#apidoc.module.mori.sort)

#### <a name="apidoc.element.mori.sort.sort"></a>[function <span class="apidocSignatureSpan">mori.</span>sort (c, e)](#apidoc.element.mori.sort.sort)
- description and source-code
```javascript
sort = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sort.a"></a>[function <span class="apidocSignatureSpan">mori.sort.</span>a (a, b)](#apidoc.element.mori.sort.a)
- description and source-code
```javascript
function a(a, b){if(D(b)){var c=rd.b?rd.b(b):rd.call(null,b),g=qd(a);ia(c,g);return D(c)}return J}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sort.b"></a>[function <span class="apidocSignatureSpan">mori.sort.</span>b (a)](#apidoc.element.mori.sort.b)
- description and source-code
```javascript
function b(a){return c.a(od,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sort.f1"></a>[function <span class="apidocSignatureSpan">mori.sort.</span>f1 (a)](#apidoc.element.mori.sort.f1)
- description and source-code
```javascript
function b(a){return c.a(od,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sort.f2"></a>[function <span class="apidocSignatureSpan">mori.sort.</span>f2 (a, b)](#apidoc.element.mori.sort.f2)
- description and source-code
```javascript
function a(a, b){if(D(b)){var c=rd.b?rd.b(b):rd.call(null,b),g=qd(a);ia(c,g);return D(c)}return J}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.sortBy"></a>[module mori.sortBy](#apidoc.module.mori.sortBy)

#### <a name="apidoc.element.mori.sortBy.sortBy"></a>[function <span class="apidocSignatureSpan">mori.</span>sortBy (c, e, f)](#apidoc.element.mori.sortBy.sortBy)
- description and source-code
```javascript
sortBy = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortBy.a"></a>[function <span class="apidocSignatureSpan">mori.sortBy.</span>a (a, b)](#apidoc.element.mori.sortBy.a)
- description and source-code
```javascript
function b(a, b){return c.c(a,od,
b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortBy.c"></a>[function <span class="apidocSignatureSpan">mori.sortBy.</span>c (a, b, c)](#apidoc.element.mori.sortBy.c)
- description and source-code
```javascript
function a(a, b, c){return sd.a(function(c,f){return qd(b).call(null,a.b?a.b(c):a.call(null,c),a.b?a.b(f):a.call(null,f))},c)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortBy.f2"></a>[function <span class="apidocSignatureSpan">mori.sortBy.</span>f2 (a, b)](#apidoc.element.mori.sortBy.f2)
- description and source-code
```javascript
function b(a, b){return c.c(a,od,
b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.sortBy.f3"></a>[function <span class="apidocSignatureSpan">mori.sortBy.</span>f3 (a, b, c)](#apidoc.element.mori.sortBy.f3)
- description and source-code
```javascript
function a(a, b, c){return sd.a(function(c,f){return qd(b).call(null,a.b?a.b(c):a.call(null,c),a.b?a.b(f):a.call(null,f))},c)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.sortedMap"></a>[module mori.sortedMap](#apidoc.module.mori.sortedMap)

#### <a name="apidoc.element.mori.sortedMap.sortedMap"></a>[function <span class="apidocSignatureSpan">mori.</span>sortedMap (a)](#apidoc.element.mori.sortedMap.sortedMap)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedMap.d"></a>[function <span class="apidocSignatureSpan">mori.sortedMap.</span>d (a)](#apidoc.element.mori.sortedMap.d)
- description and source-code
```javascript
function b(a){a=D(a);for(var b=Ng;;)if(a){var e=K(K(a)),b=Rc.c(b,G(a),Lc(a));a=e}else return b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedMap.f"></a>[function <span class="apidocSignatureSpan">mori.sortedMap.</span>f (a)](#apidoc.element.mori.sortedMap.f)
- description and source-code
```javascript
f = function (a){a=D(a);
return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.sortedMapBy"></a>[module mori.sortedMapBy](#apidoc.module.mori.sortedMapBy)

#### <a name="apidoc.element.mori.sortedMapBy.sortedMapBy"></a>[function <span class="apidocSignatureSpan">mori.</span>sortedMapBy (a, d)](#apidoc.element.mori.sortedMapBy.sortedMapBy)
- description and source-code
```javascript
function a(a, d){var e=null;if(1<arguments.length){for(var e=0,f=Array(arguments.length-1);e<f.length;)f[e]=arguments[e+1],++e;e=
new F(f,0)}return b.call(this,a,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedMapBy.d"></a>[function <span class="apidocSignatureSpan">mori.sortedMapBy.</span>d (a, b)](#apidoc.element.mori.sortedMapBy.d)
- description and source-code
```javascript
function b(a, b){for(var e=D(b),f=new Lg(qd(a),null,0,null,0);;)if(e)var g=K(K(e)),f=Rc.c(f,G(e),Lc(e)),e=g;else return f}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedMapBy.f"></a>[function <span class="apidocSignatureSpan">mori.sortedMapBy.</span>f (a)](#apidoc.element.mori.sortedMapBy.f)
- description and source-code
```javascript
f = function (a){var d=G(a);a=H(a);return b(d,a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.sortedSet"></a>[module mori.sortedSet](#apidoc.module.mori.sortedSet)

#### <a name="apidoc.element.mori.sortedSet.sortedSet"></a>[function <span class="apidocSignatureSpan">mori.</span>sortedSet (a)](#apidoc.element.mori.sortedSet.sortedSet)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedSet.d"></a>[function <span class="apidocSignatureSpan">mori.sortedSet.</span>d (a)](#apidoc.element.mori.sortedSet.d)
- description and source-code
```javascript
function b(a){return A.c(Ra,eh,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedSet.f"></a>[function <span class="apidocSignatureSpan">mori.sortedSet.</span>f (a)](#apidoc.element.mori.sortedSet.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.sortedSetBy"></a>[module mori.sortedSetBy](#apidoc.module.mori.sortedSetBy)

#### <a name="apidoc.element.mori.sortedSetBy.sortedSetBy"></a>[function <span class="apidocSignatureSpan">mori.</span>sortedSetBy (a, d)](#apidoc.element.mori.sortedSetBy.sortedSetBy)
- description and source-code
```javascript
function a(a, d){var e=null;if(1<arguments.length){for(var e=0,f=Array(arguments.length-1);e<f.length;)f[e]=arguments[e+1],++e;e=
new F(f,0)}return b.call(this,a,e)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedSetBy.d"></a>[function <span class="apidocSignatureSpan">mori.sortedSetBy.</span>d (a, b)](#apidoc.element.mori.sortedSetBy.d)
- description and source-code
```javascript
function b(a, b){return A.c(Ra,new ch(null,Rg(a),0),b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sortedSetBy.f"></a>[function <span class="apidocSignatureSpan">mori.sortedSetBy.</span>f (a)](#apidoc.element.mori.sortedSetBy.f)
- description and source-code
```javascript
f = function (a){var d=G(a);a=H(a);return b(d,a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.subseq"></a>[module mori.subseq](#apidoc.module.mori.subseq)

#### <a name="apidoc.element.mori.subseq.subseq"></a>[function <span class="apidocSignatureSpan">mori.</span>subseq (c, e, f, g, h)](#apidoc.element.mori.subseq.subseq)
- description and source-code
```javascript
subseq = function (c, e, f, g, h){switch(arguments.length){case 3:return b.call(this,c,e,f);case 5:return a.call(this,c,e,f,g,h)}throw Error("
Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subseq.c"></a>[function <span class="apidocSignatureSpan">mori.subseq.</span>c (a, b, c)](#apidoc.element.mori.subseq.c)
- description and source-code
```javascript
function b(a, b, c){var g=mh(a,b,c),h;a:{h=[Ad,Bd];var l=h.length;if(l<=Vf)for(var m=0,p=Ob(Uf);;)if(m<l)var q=m+1,p=Rb(p,h[m],null
),m=q;else{h=new $g(null,Qb(p),null);break a}else for(m=0,p=Ob(bh);;)if(m<l)q=m+1,p=Pb(p,h[m]),m=q;else{h=Qb(p);break a}h=void 0
}return t(h.call(null,b))?(a=Ib(a,c,!0),t(a)?(b=R.c(a,0,null),t(g.b?g.b(b):g.call(null,b))?
a:K(a)):null):lh.a(g,Hb(a,!0))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subseq.f3"></a>[function <span class="apidocSignatureSpan">mori.subseq.</span>f3 (a, b, c)](#apidoc.element.mori.subseq.f3)
- description and source-code
```javascript
function b(a, b, c){var g=mh(a,b,c),h;a:{h=[Ad,Bd];var l=h.length;if(l<=Vf)for(var m=0,p=Ob(Uf);;)if(m<l)var q=m+1,p=Rb(p,h[m],null
),m=q;else{h=new $g(null,Qb(p),null);break a}else for(m=0,p=Ob(bh);;)if(m<l)q=m+1,p=Pb(p,h[m]),m=q;else{h=Qb(p);break a}h=void 0
}return t(h.call(null,b))?(a=Ib(a,c,!0),t(a)?(b=R.c(a,0,null),t(g.b?g.b(b):g.call(null,b))?
a:K(a)):null):lh.a(g,Hb(a,!0))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subseq.f5"></a>[function <span class="apidocSignatureSpan">mori.subseq.</span>f5 (a, b, c, g, h)](#apidoc.element.mori.subseq.f5)
- description and source-code
```javascript
function a(a, b, c, g, h){var l=Ib(a,c,!0);if(t(l)){var m=R.c(l,0,null);return lh.a(mh(a,g,h),t(mh(a,b,c).call(null,m))?l:K(l))}return
 null}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subseq.r"></a>[function <span class="apidocSignatureSpan">mori.subseq.</span>r (a, b, c, g, h)](#apidoc.element.mori.subseq.r)
- description and source-code
```javascript
function a(a, b, c, g, h){var l=Ib(a,c,!0);if(t(l)){var m=R.c(l,0,null);return lh.a(mh(a,g,h),t(mh(a,b,c).call(null,m))?l:K(l))}return
 null}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.subvec"></a>[module mori.subvec](#apidoc.module.mori.subvec)

#### <a name="apidoc.element.mori.subvec.subvec"></a>[function <span class="apidocSignatureSpan">mori.</span>subvec (c, e, f)](#apidoc.element.mori.subvec.subvec)
- description and source-code
```javascript
subvec = function (c, e, f){switch(arguments.length){case 2:return b.call(this,c,e);case 3:return a.call(this,c,e,f)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subvec.a"></a>[function <span class="apidocSignatureSpan">mori.subvec.</span>a (a, b)](#apidoc.element.mori.subvec.a)
- description and source-code
```javascript
function b(a, b){return c.c(a,b,Q(a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subvec.c"></a>[function <span class="apidocSignatureSpan">mori.subvec.</span>c (a, b, c)](#apidoc.element.mori.subvec.c)
- description and source-code
```javascript
function a(a, b, c){return Ef(null,a,b,c,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.subvec.f2"></a>[function <span class="apidocSignatureSpan">mori.subvec.</span>f2 (a, b)](#apidoc.element.mori.subvec.f2)
- description and source-code
```javascript
function b(a, b){return c.c(a,b,Q(a))}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.subvec.f3"></a>[function <span class="apidocSignatureSpan">mori.subvec.</span>f3 (a, b, c)](#apidoc.element.mori.subvec.f3)
- description and source-code
```javascript
function a(a, b, c){return Ef(null,a,b,c,null)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.sum"></a>[module mori.sum](#apidoc.module.mori.sum)

#### <a name="apidoc.element.mori.sum.sum"></a>[function <span class="apidocSignatureSpan">mori.</span>sum (a, d, e)](#apidoc.element.mori.sum.sum)
- description and source-code
```javascript
sum = function (a, d, e){switch(arguments.length){case 0:return 0;case 1:return a;case 2:return a+d;default:var f=null;if(2<arguments.length
){for(var f=0,g=Array(arguments.length-2);f<g.length;)g[f]=arguments[f+2],++f;f=new F(g,
0)}return b.d(a,d,f)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sum.a"></a>[function <span class="apidocSignatureSpan">mori.sum.</span>a (a, b)](#apidoc.element.mori.sum.a)
- description and source-code
```javascript
a = function (a, b){return a+b}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sum.b"></a>[function <span class="apidocSignatureSpan">mori.sum.</span>b (a)](#apidoc.element.mori.sum.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sum.d"></a>[function <span class="apidocSignatureSpan">mori.sum.</span>d (b, c, d)](#apidoc.element.mori.sum.d)
- description and source-code
```javascript
function d(b, c, d){return A.c(a,b+c,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sum.f"></a>[function <span class="apidocSignatureSpan">mori.sum.</span>f (a)](#apidoc.element.mori.sum.f)
- description and source-code
```javascript
f = function (a){var b=G(a);a=K(a);var c=G(a);a=H(a);return d(b,c,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sum.f0"></a>[function <span class="apidocSignatureSpan">mori.sum.</span>f0 ()](#apidoc.element.mori.sum.f0)
- description and source-code
```javascript
f0 = function (){return 0}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sum.f1"></a>[function <span class="apidocSignatureSpan">mori.sum.</span>f1 (a)](#apidoc.element.mori.sum.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.sum.f2"></a>[function <span class="apidocSignatureSpan">mori.sum.</span>f2 (a, b)](#apidoc.element.mori.sum.f2)
- description and source-code
```javascript
f2 = function (a, b){return a+b}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.sum.l"></a>[function <span class="apidocSignatureSpan">mori.sum.</span>l ()](#apidoc.element.mori.sum.l)
- description and source-code
```javascript
l = function (){return 0}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.symbol"></a>[module mori.symbol](#apidoc.module.mori.symbol)

#### <a name="apidoc.element.mori.symbol.symbol"></a>[function <span class="apidocSignatureSpan">mori.</span>symbol (c, e)](#apidoc.element.mori.symbol.symbol)
- description and source-code
```javascript
symbol = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.symbol.a"></a>[function <span class="apidocSignatureSpan">mori.symbol.</span>a (a, b)](#apidoc.element.mori.symbol.a)
- description and source-code
```javascript
function a(a, b){var c=null!=a?[z(a),z("/"),z(b)].join(""):b;return new qc(a,b,c,null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.symbol.b"></a>[function <span class="apidocSignatureSpan">mori.symbol.</span>b (a)](#apidoc.element.mori.symbol.b)
- description and source-code
```javascript
function b(a){return a instanceof qc?a:c.a(null,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.symbol.f1"></a>[function <span class="apidocSignatureSpan">mori.symbol.</span>f1 (a)](#apidoc.element.mori.symbol.f1)
- description and source-code
```javascript
function b(a){return a instanceof qc?a:c.a(null,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.symbol.f2"></a>[function <span class="apidocSignatureSpan">mori.symbol.</span>f2 (a, b)](#apidoc.element.mori.symbol.f2)
- description and source-code
```javascript
function a(a, b){var c=null!=a?[z(a),z("/"),z(b)].join(""):b;return new qc(a,b,c,null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.take"></a>[module mori.take](#apidoc.module.mori.take)

#### <a name="apidoc.element.mori.take.take"></a>[function <span class="apidocSignatureSpan">mori.</span>take (c, e)](#apidoc.element.mori.take.take)
- description and source-code
```javascript
take = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,
c,e)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.take.a"></a>[function <span class="apidocSignatureSpan">mori.take.</span>a (a, b)](#apidoc.element.mori.take.a)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){if(0<a){var f=D(b);return f?M(G(f),c.a(a-1,H(f))):null}return null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.take.b"></a>[function <span class="apidocSignatureSpan">mori.take.</span>b (a)](#apidoc.element.mori.take.b)
- description and source-code
```javascript
function b(a){return function(b){return function(a){return function(){function c(d,g){var h=qb(a),
l=a.bb(0,a.Ra(null)-1),h=0<h?b.a?b.a(d,g):b.call(null,d,g):d;return 0<l?h:Ac(h)?h:new yc(h)}function d(a){return b.b?b.b(a):b.call
(null,a)}function l(){return b.l?b.l():b.call(null)}var m=null,m=function(a,b){switch(arguments.length){case 0:return l.call(this
);case 1:return d.call(this,a);case 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};m.l=l;m.b=d;m.a=
c;return m}()}(new Me(a))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.take.f1"></a>[function <span class="apidocSignatureSpan">mori.take.</span>f1 (a)](#apidoc.element.mori.take.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(a){return function(){function c(d,g){var h=qb(a),
l=a.bb(0,a.Ra(null)-1),h=0<h?b.a?b.a(d,g):b.call(null,d,g):d;return 0<l?h:Ac(h)?h:new yc(h)}function d(a){return b.b?b.b(a):b.call
(null,a)}function l(){return b.l?b.l():b.call(null)}var m=null,m=function(a,b){switch(arguments.length){case 0:return l.call(this
);case 1:return d.call(this,a);case 2:return c.call(this,a,b)}throw Error("Invalid arity: "+arguments.length);};m.l=l;m.b=d;m.a=
c;return m}()}(new Me(a))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.take.f2"></a>[function <span class="apidocSignatureSpan">mori.take.</span>f2 (a, b)](#apidoc.element.mori.take.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){if(0<a){var f=D(b);return f?M(G(f),c.a(a-1,H(f))):null}return null},null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.takeNth"></a>[module mori.takeNth](#apidoc.module.mori.takeNth)

#### <a name="apidoc.element.mori.takeNth.takeNth"></a>[function <span class="apidocSignatureSpan">mori.</span>takeNth (c, e)](#apidoc.element.mori.takeNth.takeNth)
- description and source-code
```javascript
takeNth = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeNth.a"></a>[function <span class="apidocSignatureSpan">mori.takeNth.</span>a (a, b)](#apidoc.element.mori.takeNth.a)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var f=
D(b);return f?M(G(f),c.a(a,Qe.a(a,f))):null},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeNth.b"></a>[function <span class="apidocSignatureSpan">mori.takeNth.</span>b (a)](#apidoc.element.mori.takeNth.b)
- description and source-code
```javascript
function b(a){return function(b){return function(c){return function(){function g(g,h){var l=c.bb(0,c.Ra(null)+1),m=Cd(l,a);return
 0===l-a*m?b.a?b.a(g,h):b.call(null,g,h):g}function h(a){return b.b?b.b(a):b.call(null,a)}function l(){return b.l?b.l():b.call(null
)}var m=null,m=function(a,b){switch(arguments.length){case 0:return l.call(this);case 1:return h.call(this,a);case 2:return g.call
(this,a,b)}throw Error("Invalid arity: "+arguments.length);
};m.l=l;m.b=h;m.a=g;return m}()}(new Me(-1))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeNth.f1"></a>[function <span class="apidocSignatureSpan">mori.takeNth.</span>f1 (a)](#apidoc.element.mori.takeNth.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(c){return function(){function g(g,h){var l=c.bb(0,c.Ra(null)+1),m=Cd(l,a);return
 0===l-a*m?b.a?b.a(g,h):b.call(null,g,h):g}function h(a){return b.b?b.b(a):b.call(null,a)}function l(){return b.l?b.l():b.call(null
)}var m=null,m=function(a,b){switch(arguments.length){case 0:return l.call(this);case 1:return h.call(this,a);case 2:return g.call
(this,a,b)}throw Error("Invalid arity: "+arguments.length);
};m.l=l;m.b=h;m.a=g;return m}()}(new Me(-1))}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeNth.f2"></a>[function <span class="apidocSignatureSpan">mori.takeNth.</span>f2 (a, b)](#apidoc.element.mori.takeNth.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var f=
D(b);return f?M(G(f),c.a(a,Qe.a(a,f))):null},null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.takeWhile"></a>[module mori.takeWhile](#apidoc.module.mori.takeWhile)

#### <a name="apidoc.element.mori.takeWhile.takeWhile"></a>[function <span class="apidocSignatureSpan">mori.</span>takeWhile (c, e)](#apidoc.element.mori.takeWhile.takeWhile)
- description and source-code
```javascript
takeWhile = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeWhile.a"></a>[function <span class="apidocSignatureSpan">mori.takeWhile.</span>a (a, b)](#apidoc.element.mori.takeWhile.a)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var f=D(b);if(f){var g;g=G(f);g=a.b?a.b(g):a.call(null,g);f=t(g)?M(G(f),c.a(a,H(f))):null}else f
=null;return f},null,null)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeWhile.b"></a>[function <span class="apidocSignatureSpan">mori.takeWhile.</span>b (a)](#apidoc.element.mori.takeWhile.b)
- description and source-code
```javascript
function b(a){return function(b){return function(){function c(f,g){return t(a.b?a.b(g):a.call(null,g))?b.a?b.a(f,g):b.call(null,
f,g):new yc(f)}function g(a){return b.b?b.b(a):b.call(null,a)}function h(){return b.l?b.l():b.call(null)}var l=null,l=function(a
,b){switch(arguments.length){case 0:return h.call(this);case 1:return g.call(this,a);case 2:return c.call(this,
a,b)}throw Error("Invalid arity: "+arguments.length);};l.l=h;l.b=g;l.a=c;return l}()}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeWhile.f1"></a>[function <span class="apidocSignatureSpan">mori.takeWhile.</span>f1 (a)](#apidoc.element.mori.takeWhile.f1)
- description and source-code
```javascript
function b(a){return function(b){return function(){function c(f,g){return t(a.b?a.b(g):a.call(null,g))?b.a?b.a(f,g):b.call(null,
f,g):new yc(f)}function g(a){return b.b?b.b(a):b.call(null,a)}function h(){return b.l?b.l():b.call(null)}var l=null,l=function(a
,b){switch(arguments.length){case 0:return h.call(this);case 1:return g.call(this,a);case 2:return c.call(this,
a,b)}throw Error("Invalid arity: "+arguments.length);};l.l=h;l.b=g;l.a=c;return l}()}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.takeWhile.f2"></a>[function <span class="apidocSignatureSpan">mori.takeWhile.</span>f2 (a, b)](#apidoc.element.mori.takeWhile.f2)
- description and source-code
```javascript
function a(a, b){return new V(null,function(){var f=D(b);if(f){var g;g=G(f);g=a.b?a.b(g):a.call(null,g);f=t(g)?M(G(f),c.a(a,H(f))):null}else f
=null;return f},null,null)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```



# <a name="apidoc.module.mori.toClj"></a>[module mori.toClj](#apidoc.module.mori.toClj)

#### <a name="apidoc.element.mori.toClj.toClj"></a>[function <span class="apidocSignatureSpan">mori.</span>toClj (c, e)](#apidoc.element.mori.toClj.toClj)
- description and source-code
```javascript
toClj = function (c, e){switch(arguments.length){case 1:return b.call(this,c);case 2:return a.call(this,c,e)}throw Error("Invalid arity: "+
arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.toClj.a"></a>[function <span class="apidocSignatureSpan">mori.toClj.</span>a (a, b)](#apidoc.element.mori.toClj.a)
- description and source-code
```javascript
function a(a, b){return Ph.d(a,Kc([Oh,b],0))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.toClj.b"></a>[function <span class="apidocSignatureSpan">mori.toClj.</span>b (a)](#apidoc.element.mori.toClj.b)
- description and source-code
```javascript
function b(a){return Ph.b(a)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.transduce"></a>[module mori.transduce](#apidoc.module.mori.transduce)

#### <a name="apidoc.element.mori.transduce.transduce"></a>[function <span class="apidocSignatureSpan">mori.</span>transduce (c, e, f, g)](#apidoc.element.mori.transduce.transduce)
- description and source-code
```javascript
transduce = function (c, e, f, g){switch(arguments.length){case 3:return b.call(this,c,e,f);case 4:return a.call(this,c,e,f,g)}throw Error("Invalid
 arity: "+arguments.length);}
```
- example usage
```shell
...
  f();
  console.log(((new Date())-s)+"ms");
}

// ~190ms V8 version 3.29.80 MBP 2.26ghz
time(function() {
  var xf = m.comp(m.map(m.inc), m.map(m.inc), m.map(m.inc));
  return m.transduce(xf, m.completing(m.sum), 0, v);
}, 10);

// ~440ms
time(function() {
  return a.map(m.inc).map(m.inc).map(m.inc).reduce(function(a,b){return a+b;}, 0);
}, 10);
'''
...
```

#### <a name="apidoc.element.mori.transduce.c"></a>[function <span class="apidocSignatureSpan">mori.transduce.</span>c (a, b, f)](#apidoc.element.mori.transduce.c)
- description and source-code
```javascript
function b(a, b, f){return c.n(a,b,b.l?b.l():b.call(null),f)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.transduce.f3"></a>[function <span class="apidocSignatureSpan">mori.transduce.</span>f3 (a, b, f)](#apidoc.element.mori.transduce.f3)
- description and source-code
```javascript
function b(a, b, f){return c.n(a,b,b.l?b.l():b.call(null),f)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.transduce.f4"></a>[function <span class="apidocSignatureSpan">mori.transduce.</span>f4 (a, b, c, g)](#apidoc.element.mori.transduce.f4)
- description and source-code
```javascript
function a(a, b, c, g){a=a.b?a.b(b):a.call(null,b);c=A.c(a,c,g);return a.b?a.b(c):a.call(null,c)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.transduce.n"></a>[function <span class="apidocSignatureSpan">mori.transduce.</span>n (a, b, c, g)](#apidoc.element.mori.transduce.n)
- description and source-code
```javascript
function a(a, b, c, g){a=a.b?a.b(b):a.call(null,b);c=A.c(a,c,g);return a.b?a.b(c):a.call(null,c)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.union"></a>[module mori.union](#apidoc.module.mori.union)

#### <a name="apidoc.element.mori.union.union"></a>[function <span class="apidocSignatureSpan">mori.</span>union (b, e, f)](#apidoc.element.mori.union.union)
- description and source-code
```javascript
union = function (b, e, f){switch(arguments.length){case 0:return bh;case 1:return b;
case 2:return a.call(this,b,e);default:var g=null;if(2<arguments.length){for(var g=0,h=Array(arguments.length-2);g<h.length;)h[g
]=arguments[g+2],++g;g=new F(h,0)}return c.d(b,e,g)}throw Error("Invalid arity: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.union.a"></a>[function <span class="apidocSignatureSpan">mori.union.</span>a (a, b)](#apidoc.element.mori.union.a)
- description and source-code
```javascript
function a(a, b){return Q(a)<Q(b)?A.c(Nc,b,a):A.c(Nc,a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.union.b"></a>[function <span class="apidocSignatureSpan">mori.union.</span>b (a)](#apidoc.element.mori.union.b)
- description and source-code
```javascript
b = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.union.d"></a>[function <span class="apidocSignatureSpan">mori.union.</span>d (a, c, d)](#apidoc.element.mori.union.d)
- description and source-code
```javascript
function b(a, c, d){a=Qh(Q,Nc.d(d,c,Kc([a],0)));return A.c(af,G(a),H(a))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.union.f"></a>[function <span class="apidocSignatureSpan">mori.union.</span>f (a)](#apidoc.element.mori.union.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=H(a);return b(c,d,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.union.f0"></a>[function <span class="apidocSignatureSpan">mori.union.</span>f0 ()](#apidoc.element.mori.union.f0)
- description and source-code
```javascript
f0 = function (){return bh}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.union.f1"></a>[function <span class="apidocSignatureSpan">mori.union.</span>f1 (a)](#apidoc.element.mori.union.f1)
- description and source-code
```javascript
f1 = function (a){return a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.union.f2"></a>[function <span class="apidocSignatureSpan">mori.union.</span>f2 (a, b)](#apidoc.element.mori.union.f2)
- description and source-code
```javascript
function a(a, b){return Q(a)<Q(b)?A.c(Nc,b,a):A.c(Nc,a,b)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.union.l"></a>[function <span class="apidocSignatureSpan">mori.union.</span>l ()](#apidoc.element.mori.union.l)
- description and source-code
```javascript
l = function (){return bh}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.updateIn"></a>[module mori.updateIn](#apidoc.module.mori.updateIn)

#### <a name="apidoc.element.mori.updateIn.updateIn"></a>[function <span class="apidocSignatureSpan">mori.</span>updateIn (e, h, l, m, p, q, s)](#apidoc.element.mori.updateIn.updateIn)
- description and source-code
```javascript
updateIn = function (e, h, l, m, p, q, s){switch(arguments.length){case 3:return d.call(this,e,h,l);case 4:return c.call(this,e,h,l,m);case 5:return
 b.call(this,e,h,l,m,p);case 6:return a.call(this,e,h,l,m,p,q);default:var u=null;if(6<arguments.length){for(var u=0,v=Array(arguments
.length-6);u<v.length;)v[u]=arguments[u+6],++u;u=new F(v,0)}return f.d(e,h,l,m,p,q,u)}throw Error("Invalid arity: "+arguments.length
);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.P"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>P (a, b, c, d, f, q)](#apidoc.element.mori.updateIn.P)
- description and source-code
```javascript
function a(a, b, c, d, f, q){var s=R.c(b,0,null);return(b=Ed(b))?Rc.c(a,s,e.P(S.a(a,s),b,c,d,f,q)):Rc.c(a,s,
function(){var b=S.a(a,s);return c.n?c.n(b,d,f,q):c.call(null,b,d,f,q)}())}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.c"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>c (a, b, c)](#apidoc.element.mori.updateIn.c)
- description and source-code
```javascript
function d(a, b, c){var d=R.c(b,0,null);return(b=Ed(b))?Rc.c(a,d,e.c(S.a(a,d),b,c)):Rc.c(a,d,function(){var b=
S.a(a,d);return c.b?c.b(b):c.call(null,b)}())}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.d"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>d (a, c, d, f, g, h, v)](#apidoc.element.mori.updateIn.d)
- description and source-code
```javascript
function b(a, c, d, f, g, h, v){var y=R.c(c,0,null);return(c=Ed(c))?Rc.c(a,y,T.d(e,S.a(a,y),c,d,f,Kc([g,h,v],0))):Rc.c(a,y,T.d(d,S.a(a
,y),f,g,h,Kc([v],0)))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.f"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>f (a)](#apidoc.element.mori.updateIn.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=K(a);var e=G(a);a=K(a);var f=G(a);a=K(a);var g=
G(a);a=K(a);var v=G(a);a=H(a);return b(c,d,e,f,g,v,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.f3"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>f3 (a, b, c)](#apidoc.element.mori.updateIn.f3)
- description and source-code
```javascript
function d(a, b, c){var d=R.c(b,0,null);return(b=Ed(b))?Rc.c(a,d,e.c(S.a(a,d),b,c)):Rc.c(a,d,function(){var b=
S.a(a,d);return c.b?c.b(b):c.call(null,b)}())}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.f4"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>f4 (a, b, c, d)](#apidoc.element.mori.updateIn.f4)
- description and source-code
```javascript
function c(a, b, c, d){var f=R.c(b,0,null);return(b=Ed(b))?Rc.c(a,f,e.n(S.a(a,f),b,c,d)):Rc.c(a,f,function(){var b=S.a(a,f);return
c.a?c.a(b,d):c.call(null,b,d)}())}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.f5"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>f5 (a, b, c, d, f)](#apidoc.element.mori.updateIn.f5)
- description and source-code
```javascript
function b(a, b, c, d, f){var q=R.c(b,0,null);return(b=Ed(b))?Rc.c(a,q,e.r(S.a(a,q),b,c,d,f)):Rc.c(a,q,function(){var b=S.a(a,q);return
 c.c?c.c(b,d,f):c.call(null,b,d,f)}())}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.f6"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>f6 (a, b, c, d, f, q)](#apidoc.element.mori.updateIn.f6)
- description and source-code
```javascript
function a(a, b, c, d, f, q){var s=R.c(b,0,null);return(b=Ed(b))?Rc.c(a,s,e.P(S.a(a,s),b,c,d,f,q)):Rc.c(a,s,
function(){var b=S.a(a,s);return c.n?c.n(b,d,f,q):c.call(null,b,d,f,q)}())}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.n"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>n (a, b, c, d)](#apidoc.element.mori.updateIn.n)
- description and source-code
```javascript
function c(a, b, c, d){var f=R.c(b,0,null);return(b=Ed(b))?Rc.c(a,f,e.n(S.a(a,f),b,c,d)):Rc.c(a,f,function(){var b=S.a(a,f);return
c.a?c.a(b,d):c.call(null,b,d)}())}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.updateIn.r"></a>[function <span class="apidocSignatureSpan">mori.updateIn.</span>r (a, b, c, d, f)](#apidoc.element.mori.updateIn.r)
- description and source-code
```javascript
function b(a, b, c, d, f){var q=R.c(b,0,null);return(b=Ed(b))?Rc.c(a,q,e.r(S.a(a,q),b,c,d,f)):Rc.c(a,q,function(){var b=S.a(a,q);return
 c.c?c.c(b,d,f):c.call(null,b,d,f)}())}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.varyMeta"></a>[module mori.varyMeta](#apidoc.module.mori.varyMeta)

#### <a name="apidoc.element.mori.varyMeta.varyMeta"></a>[function <span class="apidocSignatureSpan">mori.</span>varyMeta (f, l, m, p, q, s, u)](#apidoc.element.mori.varyMeta.varyMeta)
- description and source-code
```javascript
varyMeta = function (f, l, m, p, q, s, u){switch(arguments.length){case 2:return e.call(this,f,l);case 3:return d.call(this,f,l,m);case 4:return
c.call(this,f,l,m,p);case 5:return b.call(this,f,l,m,p,q);case 6:return a.call(this,f,l,m,p,q,s);default:var v=null;if(6<arguments
.length){for(var v=
0,y=Array(arguments.length-6);v<y.length;)y[v]=arguments[v+6],++v;v=new F(y,0)}return g.d(f,l,m,p,q,s,v)}throw Error("Invalid arity
: "+arguments.length);}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.P"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>P (a, b, c, d, e, f)](#apidoc.element.mori.varyMeta.P)
- description and source-code
```javascript
function a(a, b, c, d, e, f){var g=O,v=Vc(a);b=b.r?b.r(v,c,d,e,f):b.call(null,v,c,d,e,f);return g(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.a"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>a (a, b)](#apidoc.element.mori.varyMeta.a)
- description and source-code
```javascript
function e(a, b){var c=O,d;d=Vc(a);d=b.b?b.b(d):b.call(null,d);return c(a,d)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.c"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>c (a, b, c)](#apidoc.element.mori.varyMeta.c)
- description and source-code
```javascript
function d(a, b, c){var d=O,e=Vc(a);b=b.a?b.a(e,c):b.call(null,e,c);return d(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.d"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>d (a, c, d, e, f, g, h)](#apidoc.element.mori.varyMeta.d)
- description and source-code
```javascript
function b(a, c, d, e, f, g, h){return O(a,T.d(c,Vc(a),d,e,f,Kc([g,h],0)))}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.f"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>f (a)](#apidoc.element.mori.varyMeta.f)
- description and source-code
```javascript
f = function (a){var c=G(a);a=K(a);var d=G(a);a=K(a);var e=G(a);a=K(a);var f=G(a);a=K(a);var g=G(a);a=K(a);var h=G(a);a=H(a);return
b(c,d,e,f,g,h,a)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.f2"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>f2 (a, b)](#apidoc.element.mori.varyMeta.f2)
- description and source-code
```javascript
function e(a, b){var c=O,d;d=Vc(a);d=b.b?b.b(d):b.call(null,d);return c(a,d)}
```
- example usage
```shell
...
}

// ~70ms
for(var j = 0; j < 10; j++) {
  s = new Date();
  var mv = m.mutable.thaw(m.vector());
  for(var i = 0; i < 10000000; i++) {
    mv = m.mutable.conj.f2(mv, i);
  }
  var v = m.mutable.freeze(mv);
  print("Mutable vector conj " + m.count(v) + " items " + ((new Date())-s));
  gc();
}
'''
...
```

#### <a name="apidoc.element.mori.varyMeta.f3"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>f3 (a, b, c)](#apidoc.element.mori.varyMeta.f3)
- description and source-code
```javascript
function d(a, b, c){var d=O,e=Vc(a);b=b.a?b.a(e,c):b.call(null,e,c);return d(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.f4"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>f4 (a, b, c, d)](#apidoc.element.mori.varyMeta.f4)
- description and source-code
```javascript
function c(a, b, c, d){var e=O,f=Vc(a);b=b.c?b.c(f,c,d):b.call(null,f,c,d);return e(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.f5"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>f5 (a, b, c, d, e)](#apidoc.element.mori.varyMeta.f5)
- description and source-code
```javascript
function b(a, b, c, d, e){var f=O,g=Vc(a);b=b.n?b.n(g,
c,d,e):b.call(null,g,c,d,e);return f(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.f6"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>f6 (a, b, c, d, e, f)](#apidoc.element.mori.varyMeta.f6)
- description and source-code
```javascript
function a(a, b, c, d, e, f){var g=O,v=Vc(a);b=b.r?b.r(v,c,d,e,f):b.call(null,v,c,d,e,f);return g(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.n"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>n (a, b, c, d)](#apidoc.element.mori.varyMeta.n)
- description and source-code
```javascript
function c(a, b, c, d){var e=O,f=Vc(a);b=b.c?b.c(f,c,d):b.call(null,f,c,d);return e(a,b)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.varyMeta.r"></a>[function <span class="apidocSignatureSpan">mori.varyMeta.</span>r (a, b, c, d, e)](#apidoc.element.mori.varyMeta.r)
- description and source-code
```javascript
function b(a, b, c, d, e){var f=O,g=Vc(a);b=b.n?b.n(g,
c,d,e):b.call(null,g,c,d,e);return f(a,b)}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mori.vector"></a>[module mori.vector](#apidoc.module.mori.vector)

#### <a name="apidoc.element.mori.vector.vector"></a>[function <span class="apidocSignatureSpan">mori.</span>vector (a)](#apidoc.element.mori.vector.vector)
- description and source-code
```javascript
function a(a){var d=null;if(0<arguments.length){for(var d=0,e=Array(arguments.length-0);d<e.length;)e[d]=arguments[d+0],++d;d=new
 F(e,0)}return b.call(this,d)}
```
- example usage
```shell
...
You can use it from your projects like so:

'''javascript
var inc = function(n) {
  return n+1;
};

mori.intoArray(mori.map(inc, mori.vector(1,2,3,4,5)));
// => [2,3,4,5,6]
'''

Efficient non-destructive updates!

'''javascript
var v1 = mori.vector(1,2,3);
...
```

#### <a name="apidoc.element.mori.vector.d"></a>[function <span class="apidocSignatureSpan">mori.vector.</span>d (a)](#apidoc.element.mori.vector.d)
- description and source-code
```javascript
function b(a){if(a instanceof F&&0===a.m)a:{a=a.e;var b=a.length;if(32>b)a=new W(null,b,5,uf,a,null);else{for(var e=32,f=(new W(
null,32,5,uf,a.slice(0,32),null)).$a(null);;)if(e<b)var g=e+1,f=de.a(f,a[e]),e=g;else{a=Qb(f);break a}a=void 0}}else a=zf(a);return
 a}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mori.vector.f"></a>[function <span class="apidocSignatureSpan">mori.vector.</span>f (a)](#apidoc.element.mori.vector.f)
- description and source-code
```javascript
f = function (a){a=D(a);return b(a)}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
