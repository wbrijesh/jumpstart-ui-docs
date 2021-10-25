---
sidebar_position: 1
---

# Navbar

Buttons allow users to take actions, and make choices, with a single tap.

![Locale Dropdown](/img/tutorial/jumpstart-ui-button.png)

```jsx title="Import Button component"
import { Navbar } from "jumpstart-ui";
```

```jsx title="Button Component"
<Navbar
  appLogo="https://assets.brijesh-wawdhane.com/jumpstart-ui-logo.svg"
  appName="Jumpstart UI"
  buttonBlankTitles={[
    'Documentation',
    'Github'
  ]}
  buttonBlankUrls={[
    'https://google.com',
    'https://github.com'
  ]}
  buttonFilledTitle="Get Started"
  buttonFilledUrl="https://brijesh-wawdhane.com"
  height="16"
  homePageUrl="https://brijesh-wawdhane.com"
  onClick={() => {}}
/>
```

```jsx
<Disclosure as="nav" className="bg-white border-b border-gray-200">
    {({ open }) => (
    <>
        <div className="max-w-full mx-auto px-4 sm:px-6 lg:px-6">
        {/* Default Height - h-16 */}
        <div className={`flex justify-between h-16`}>
            <div className="flex">
            <div className="-ml-2 mr-2 flex items-center md:hidden">
                <Disclosure.Button className="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white">
                <span className="sr-only">Open main menu</span>
                {open ? (
                    <XIcon className="block h-6 w-6" aria-hidden="true" />
                ) : (
                    <MenuIcon className="block h-6 w-6" aria-hidden="true" />
                )}
                </Disclosure.Button>
            </div>
            {/* App's name homepage url */}
            <div className="flex-shrink-0 flex items-center">
                <a href='#' className="flex-shrink-0">
                <h2 className="text-xl text-gray-900 font-semibold">
                    App Name
                </h2>
                </a>
            </div>
            </div>
            <div className="flex items-center">
            <div className="flex-shrink-0">
            {/* Mobile CTA Button */}
                <a href="#">
                <button
                    type="button"
                    className="relative md:invisible inline-flex items-center px-3 py-1.5 border border-transparent text-base font-medium rounded text-white bg-blue-600 shadow-sm hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500"
                >
                    <span>CTA Button</span>
                </button>
                </a>
            </div>
            <div className="hidden md:ml-4 md:flex-shrink-0 md:flex md:items-center">
                <Menu as="div" className="ml-3 relative">
                <div className="hidden md:ml-6 md:flex md:items-center md:space-x-4">
                    {/* Desktop Navigation Button */}
                    <a href="#" type="button">
                        <span className="mr-4 relative inline-flex items-center px-2 py-1 border border-transparent text-base font-medium rounded text-gray-600 bg-transparent shadow-none hover:text-gray-900 hover:bg-gray-200 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-400">
                        One
                        </span>
                    </a>
                    <a href="#">
                    <button
                        type="button"
                        className="relative hidden:onlyMobile inline-flex items-center px-3 py-1.5 border border-transparent text-base font-medium rounded text-white bg-blue-600 shadow-sm hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500"
                    >
                    {/* Desktop CTA Button */}
                        <span>CTA Button</span>
                    </button>
                    </a>
                </div>
                </Menu>
            </div>
            </div>
        </div>
        </div>

        <Disclosure.Panel className="md:hidden">
        {/* Mobile Navigation Button */}
        <div className="px-2 pt-2 pb-3 space-y-1 sm:px-3">
            <a
                href="#"
                className="text-gray-600 hover:bg-blue-500 hover:text-white block px-3 py-2 rounded-md text-base font-medium"
            >
                One
            </a>
        </div>
        </Disclosure.Panel>
    </>
    )}
</Disclosure>
```

| Argument | Options                    |
| -------- | -------------------------- |
| link     | link                       |
| size     | `small`, `medium`, `large` |
| title    | Button Label               |
| variant  | `primary`, `ghost`         |




