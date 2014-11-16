ERRORS
======

This is a file where I store some error messages, so I can solve those faster next time.

Error: readline not linked / a program was installed by two different tools
(rails was installed by rbenv and homebrew in different versions - linking error)

Messages

$ rake migrate
rake aborted!
LoadError: dlopen(/Users/ben/.rbenv/versions/2.1.5/lib/ruby/2.1.0/x86_64-darwin14.0/readline.bundle, 9): Library not loaded: @@HOMEBREW_PREFIX@@/opt/readline/lib/libreadline.6.dylib
  Referenced from: /Users/ben/.rbenv/versions/2.1.5/lib/ruby/2.1.0/x86_64-darwin14.0/readline.bundle

Solution

brew uninstall (program)
brew uninstall readline
brew install readline
brew link --force readline
