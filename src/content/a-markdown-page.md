---
layout: page
title: 'Example Markdown page'
---

Now we're writing in Markdown! Pretty nice, huh?

This starter has out-of-the-box support for basic Markdown rendering. The `content/` directory is where you put all of your Markdown content in. Gatsby will build your pages out of it. Gatsby will also follow the directory structure of your files too, so when you store a page at e.g. `content/projects/large-hadron-collider.md`, it will be built in `/projects/large-hadron-collider/`.

[That's cool! Okay, take me back home.](/)

## Page.tsx

```tsx
import * as React from 'react';
import styled from '@emotion/styled';

import { dimensions } from '../styles/variables';

const StyledPage = styled.div`
  display: block;
  flex: 1;
  position: relative;
  padding: ${dimensions.containerPadding}rem;
  margin-bottom: 3rem;
`;

interface PageProps {
  className?: string;
}

const Page: React.FC<PageProps> = ({ children, className }) => (
  <StyledPage className={className}>{children}</StyledPage>
);

export default Page;
```
