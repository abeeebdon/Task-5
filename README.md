This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
#   T a s k - 5 
 
 

npx serve@latest out

<div className=" relative bg-lpurple basis-[80%]">
          <div className="w-[193px] h-[193px] pt-[61px] pb-[60px]  rounded-lg text-center  flex flex-col justify-center items-center">
            <div
              className={`my-2 basis-[80%] ${
                imageUrl ? 'bg-white' : 'bg-purple'
              }  `}
            >
              {!imageUrl && (
                <Image
                  src="/images/upload.svg"
                  alt="upload"
                  width={40}
                  height={40}
                />
              )}
            </div>
            <p className="paragraph font-[600] text-purple">
              {imageUrl ? 'Change Image' : '+ Upload Image'}
            </p>
          </div>
         
          {imageUrl && (
            <div className="absolute w-full h-full opacity-1 cursor-pointer">
              <Image src={imageUrl} width={193} height={193} alt="Profile" />
            </div>
          )}
        </div>
        <p className="label text-gray  ">
          Image must be below 1024x1024px. Use PNG or JPG format.
        </p>

import React, { useState } from 'react';

const options = [
{ value: 'option1', label: 'Option 1', imageUrl: '/path/to/image1.png' },
{ value: 'option2', label: 'Option 2', imageUrl: '/path/to/image2.png' },
// Add more options as needed
];

const CustomDropdown = () => {
const [selectedOption, setSelectedOption] = useState(options[0]);

return (

);
};

export default CustomDropdown;
