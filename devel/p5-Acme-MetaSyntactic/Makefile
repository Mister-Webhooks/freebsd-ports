PORTNAME=	Acme-MetaSyntactic
PORTVERSION=	1.015
CATEGORIES=	devel perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	Themed metasyntactic variables names
WWW=		https://metacpan.org/release/Acme-MetaSyntactic

LICENSE=	ART10 GPLv1+
LICENSE_COMB=	dual
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${RUN_DEPENDS}
RUN_DEPENDS=	p5-libwww>=0:www/p5-libwww

USES=		perl5
USE_PERL5=	configure

NO_ARCH=	yes

PORTSCOUT=	skipv:3rd_rock-0.001

.include <bsd.port.mk>
