# Click 'n' Clone 
A bookmarklet for rapid repo cloning.

Drag this link to your bookmarks bar: <a href="javascript:(function()%7Bjavascript%3A(function()%7B%0A%20%20%20%20var%20serverUrl%20%3D%20'http%3A%2F%2F127.0.0.1%3A5000%2Fclone'%3B%0A%20%20%20%20var%20currentUrl%20%3D%20window.location.href%3B%0A%20%20%20%20var%20match%20%3D%20currentUrl.match(%2F%5Ehttps%3F%3A%5C%2F%5C%2Fgithub%5C.com%5C%2F(%5B%5E%5C%2F%5D%2B%5C%2F%5B%5E%5C%2F%5D%2B)%2F)%3B%0A%20%20%20%20if%20(match)%20%7B%0A%20%20%20%20%20%20%20%20var%20repoUrl%20%3D%20'https%3A%2F%2Fgithub.com%2F'%20%2B%20match%5B1%5D%20%2B%20'.git'%3B%0A%20%20%20%20%20%20%20%20window.location.href%20%3D%20serverUrl%20%2B%20'%3Furl%3D'%20%2B%20encodeURIComponent(repoUrl)%3B%0A%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20%20%20alert('This%20doesn%5C't%20appear%20to%20be%20a%20GitHub%20repository%20page.')%3B%0A%20%20%20%20%7D%0A%7D)()%3B%7D)()%3B">gitclone</a>

