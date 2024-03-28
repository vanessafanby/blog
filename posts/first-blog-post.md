---
title: This is my first blog post!
published_at: 2022-11-04T15:00:00.000Z
snippet: This is an excerpt of my first blog post.
---

Hello, world!

Today is my first day at RMIT digital media. I met lots of new friends including Silvia, Julie and Juliet. I was in a group with Oscar and Zoe for scavenger hunt, we had a tough time finding places and items.
"$gfm": "https://deno.land/x/gfm@0.1.26/mod.ts"
import { CSS, render } from "$gfm";
import { Head } from "$fresh/runtime.ts";
export default function PostPage(props: PageProps<Post>) {
  const post = props.data;
  return (
    <>
      <Head>
        <style dangerouslySetInnerHTML={{ __html: CSS }} />
      </Head>
      // ...
      <div
        class="mt-8 markdown-body"
        dangerouslySetInnerHTML={{ __html: render(post.content) }}
      />
    </>
  );
}

# This is h1

## This is h2

_underline_

**bold**


