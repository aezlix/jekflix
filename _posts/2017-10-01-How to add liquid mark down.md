---
published: false
---
---
layout: post
title: "How (1)"
description: How to add Liquid-Markdown to your site?
image: 'https://i.github-camo.com/a0aac6109b3299d855711c188cfdf9453343577a/687474703a2f2f6f70656e736f757263652e6f6c697665726d616b2e65732f696d616765732f323031362d30332d32392d6e6577626f756e642d6461726b2d6d642e706e67'
category: 'blog' 'how'
twitter_text: Lorem ipsum dolor sit amet, consectetur adipisicing elit.
introduction: Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
---

# What is it?

- Combines Liquid and extended Markdown (via Kramdown) for customer-safe templating of Rails pages and emails
- Integrates with Panoramic to add ActiveRecord database storage of templates for editing
- Generates both plain text and html parts of an email from a single template (replacing other markdown email gems)
- Supports html layouts for emails (unlike other markdown email gems)

# Who made it?

## Liquid Markdown was made by [Buzzware](https://github.com/buzzware) on Oct 3, 2016

# A piece of this 

'''
require 'liquid_markdown/resolver' # required

class TemplateStorage < ActiveRecord::Base
  store_templates

  # required
  def self.resolver(options={})
    LiquidMarkdown::Resolver.using self, options
  end
end

'''

### Thanks for reading, check the [site](http://test.athelo.net/jekflix) for more




