# Talk Ideas:
CRB 17-Feb-2014

## When not to ruby
[repo](https://github.com/dapplebeforedawn/patterns-of-failure)

A talk about when you might choose a langauge other than ruby.


## Horse e-books-motron
[repo](https://github.com/dapplebeforedawn/horse-ebooks-talk)

A talk about using golang's concurrency primitives to build up a complex chat room application that includes AI.

## Developer Honypot
> Refactoring code that your devops wrote.

This talk would be more of a performance-art piece.  What I think is interesting here is that one simple text file can kill CMM productivity for an afternoon.  Does that translate to talk-form?

## It's your problem now.
> How to take ownership of someone else's code base.

This idea is half baked, but I was just thinking about what I do when looking at someone's code.

1. Open VIM and `:r !tree -f`
2. Start at the top level test and then walk down through the routes -> controllers -> models
3. Run ctags

I've see you dig right into the unit tests.  There might be something interesting here.

## How to do code review
Basically a summary of what we've been doing for Ryan/Zach/Dr. Ryan.  Would end up being a really similar talk to "It's your problem now".

## VIM Pro-tips.
If we do this one, I want to challenge the audience.  I bet we can promise them that every single person will learn something new.  Also we would need to find a way to make it engaging, even if you're not a true believer.  Perhaps we could make some kind of game out of it, or tell a story?

Vanilla VIM only.  No plugins.

I know not everyone uses VIM at CRB, so this would need to have a slight 'why you should use VIM' slant.  Just a touch.

1. VIM and the commandline, VIM's secret weapon
  1. `:r !tree`
  2. `:w !pbcopy`
  3. `git diff | vim -`

1. Mapping leader keys
  1. `:map <leader>t !rspec %<cr>`
  2. `:map <leader>r !touch tmp/restart<cr>`

1. Going places
  1.  using `^Wgf` to open files
  2.  The jump stack `^I` and `^O`
  3.  `*` and `#` and `%`
  4.  `^6`
  5.  `f` and `F` and `;`
  6.  `^O`
  7.  `^[` in insert mode
  7.  Omnicomplete `^N`, `^P`

1. CTags Integration
  1. `^T`, `^[`, `^[`

1. The quickfix
  1. filename:linenum:comment
  2. `cg quickfix.out` `cw`
  3. `cex system('ack something`)

1. Command mode and Searching
  1. `q:` and `^F` 
  2. `q/`
  3. `%`, `^R%`
  4. `^R^W`, `^R^A`

1. Tab and Window Management
  1. `vsp`, `sp` `^W`
  2. `:map <leader>r :bel new \| setl bt=nofile \| r !bc your_file <cr>`

1. Visual block mode
  1. `^V` `I`

1. Replacing text
  1. `s`
  2. `r`, `R`
  3. `xp`
  4. `d`
  5. `c`
  6. `~`

1. Opening a document from the web
  1. `:e http://www.google.com`

1. Trailing whitespace is shitty
  1. `set listchars=trail:💩` 

1. Fixing a shell command
  1. `^X^E` at the prompt to edit the command in `$EDITOR`
  2. `fc` to edit the last command in `$EDITOR`
