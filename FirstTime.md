# First-Time Git Setup

## Your Identity

```bash
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

## Generating a new SSH key

```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
eval $(ssh-agent -s)
ssh-add ~/.ssh/id_rsa
```

Press ENTER for default

## Adding a new SSH key to your GitHub account

```bash
clip < ~/.ssh/id_rsa.pub
```

Your account -> Settings -> SSH and GPG keys -> New SSH key or Add SSH key -> paste

## Testing

```bash
ssh -T git@github.com
 ```

You've successfully authenticated, but GitHub does not provide shell access.
